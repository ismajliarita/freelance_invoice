A freelancer logs in, tracks time against client projects, turns that time into invoices, sends them, and records payments. It’s the best pick for teaching money handling, immutability, and document generation — three things most juniors have never touched.

Functional Requirements
General requirements:
	Register: Allow the user to create an account
	Log-in: The user will give their credentials to access the system
	Log out: Allow a user to securely end their session
	View account: Allow a user to view their account information
	Edit account: Allow a user to update their account information
Client Management
	Create client
	View clients
	View client details
	Edit client
	Delete client
Project Management
	Create project for a client
	View projects
	View project details
	Edit project
	Delete project
Time Tracking
	Create time entry for a project
	View time entries
	Edit time entry
	Delete time entry
	Mark time as billable/non-billable
Invoice Management
	Create invoice from billable time
	View invoices
	View invoice details
	Edit invoice while in draft
	Send invoice to client
	Change invoice status
	Prevent modification of issued invoices
Payment Management
	Record payment
	View payments
	View outstanding invoice balance
	Track paid, unpaid, and partially paid invoices
Document Generation
	Generate invoice as a document/PDF
	Download generated invoice

Possible
	Send invoice once project is done

Non-Functional Requirements
	Security
	Performance
	Reliability
	Data integrity
	Usability
	Maintainability
	Scalability
	Availability
	Compatibility
	Testability


Freelancer Workspace
	A workspace for freelancers to manage clients, projects, work, finances, and client collaboration.
		Dashboard
			active projects
			active invoices (not paid yet)
			anything still not done, open or active 
		Clients
			profile management,
			invitation for new client profiles/accounts
			ties to projects, milestones, deadlines for deliverables
		Projects
			Invoice
			Files
			Communication line with client
			Tasks
				defined type of task, so it can be defined regarding time tracking and invoicing 
			Milestones
				like deliverables
			KPIs (kinda like time tracking?)
		Time Tracking
			Tasks
			definition of hours and how much an hour gets paid
				hours of development vs analysis vs testing and stuff are different
		Invoices and Payments
			based on time tracking and task type.
				one type of task costs a defined amount which can be adjusted or customized for each project
		Client collaboration
			like chat requests. not direct line of communication like whatsapp
	
Marketplace
	Freelancer search/discovery
	Profiles - like dashboards for freelancers
	job postings
	biddings
	