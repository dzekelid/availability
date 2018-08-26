---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}:
    get:
      summary: Returns a list of available times.
      description: "Choose your search criteria carefully. Availability is an expensive
        call. If you search availability for all resources\r\nthen you should only
        do so for a single date. If you decide to search availability for multiple
        dates you should only do so\r\nfor a specific resource by specifying the optional
        resourceId parameter.\r\n\r\nStart and End times are specified as military
        times e.g. 800 = 8:00am, 2230 = 10:30pm. \r\nYou will only see availability
        within the boundary of your business start and end times.\r\n\r\ndayAvailability
        will return day availablility for the number of days requested from the start
        date.\r\n\r\nfirstDayAvailable only works with day availability. If set to
        true it will look for the first day available within the range specified\r\nby
        the dayAvailability parameter. The two parameters together can be a clever
        way to display availability for a week or month.\r\nTip - pass in the beginning
        of the week or month, and available times are displayed for the first available
        date if exists.\r\n\r\nYou should only specify the duration parameter if you
        let your customers choose the duration of the appointment. e.g. from a list.\r\n\r\nThe
        tz parameter allows you to select a suitable timezone for the customer to
        book in. Your app should be timezone aware if you \r\nuse this option. The
        requested timezone is specified as an offset(plus or minus) from GMT time."
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddate-get
      parameters:
      - in: query
        name: dayAvailability
        description: Return day availability for number of days specified
      - in: query
        name: duration
        description: Duration of the service if different than the default
      - in: path
        name: endDate
        description: End Date for availability search
      - in: query
        name: endTime
        description: End Time for availability search
      - in: query
        name: firstDayAvailable
        description: Return available times for the first available day
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceGroupId
        description: Resource Group Id for availability search
      - in: query
        name: resourceId
        description: Resource Id for availability search
      - in: query
        name: resourceIds
        description: Comma separated Resource Ids for availability search
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for availability search
      - in: query
        name: startTime
        description: Start Time for availability search
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}/days:
    get:
      summary: Returns a list of available days.
      description: "This end point is used to show day level availability. For example
        if the business is closed, or there is a public holiday.\r\n\r\nDay level
        availability is a good way to restrict your choices of dates in your app and
        improve usability."
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateDaysGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddatedays-get
      parameters:
      - in: path
        name: endDate
        description: End Date for availability search
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceId
        description: Resource Id to filter on
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for availability search
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
      - Days
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}/unavailable:
    get:
      summary: Returns a list of unavailable times.
      description: This endpoint is used to show unavailable times and provides information
        why the timeslot is unavailable.
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateUnavailableGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddateunavailable-get
      parameters:
      - in: query
        name: duration
        description: Duration of the service if different than the default
      - in: path
        name: endDate
        description: End Date for unavailable time search
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceId
        description: Resource Id to filter on
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for unavailable time search
      - in: query
        name: tzOffset
        description: Request timezone offset to view unavailable times
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
      - Unavailable
  /consumer/v1/availability/{appointmentId}/reschedule:
    get:
      summary: Returns a list of available times.
      description: "This end point is used to find availability for the purpose of
        rescheduling an appointment.\r\nAvailability defaults to the serviceId, resourceId
        and timezone from the original appointment.\r\nAfter choosing from the availability,
        you can call the appointment reschedule endpoint."
      operationId: ConsumerV1AvailabilityByAppointmentIdRescheduleGet
      x-api-path-slug: consumerv1availabilityappointmentidreschedule-get
      parameters:
      - in: path
        name: appointmentId
        description: Appointment Id of the original appointment being rescheduled
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - AppointmentId
      - Reschedule
---