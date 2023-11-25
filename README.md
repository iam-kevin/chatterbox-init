# ChatterBox

This is a repository to help me gain confidence in building in [Go](https://go.dev/), and working with [Cloud-native](https://www.ibm.com/topics/cloud-native) Infrastructure. 

## About the project

I'll be building a chat service that will do the following:

- Allow users to be created using a username. upon creation, you'll be prompted to add in a name and a NIDA-like information as well as prompting them to create a 4-digit pin.
- Allow users to join room by typing `/join <chatroom-id>`
- In the chatroom, the users can send money to others by typing `/send <username> <amount>`, to confirm the transfer, they user will need to authorize by typing in their 4-digit pin.
- Users can leave the chat room by typing `/leave`

## How I intent to go about this

[This excalidraw link](https://link.excalidraw.com/readonly/vdjg14CL0Tqg4YGe2K0T) shows a simple structure of how I intent to go about this. I'm sure there are better ways around this, But this setup is helpful for me to learn the things I want right now.
Quick TLDR, I'll be creating 3 things
- `ChatterBox`  service, which is a service to manage the chatrooms and users
- `KYC` service, which would house all personal identifying information
- `ChatterBox Web` app, which is how the users would interact with the system.

### Technologies

For the purpose of learning, 
- the services (Chatterbox and KYC) will be developed in [Go](https://go.dev/)
- The web app will be developed in [React 18](https://react.dev/) using [Vite tooling](https://vitejs.dev/)
- Database used will be [PostgreSQL 15+](https://www.postgresql.org/)

### Deployments

The entire project will HAVE to be able to run locally first. Then moving to cloud deployments:
- The services will be deployed in either [Fly.io](https://fly.io/) or [Linode](https://www.linode.com/) 
- The web app will be deployed over at [Vercel](https://vercel.com/)
- The database will be using [Neon](https://neon.tech/) or [Supabase](https://supabase.com/database)

### Bonus
- To learn K8s and Docker properly, this project _might_ also be setup to work in those environemnts

## Timelines

This would a slow journey, especially because I'll be building this in a from the free time I am able to get after work. I'll like to have completed this by **this year**, but I'll be updating this documentation rather frequently, to reflect the active changes will be reflected on this [Trello board](https://trello.com/b/2rrn0a2z/chatterbox)

## Contributions

This project isn't set up for code contirbutions (yet? _maybe_). But to feel free to chat / comment / critic things here. And when I have the energy / time, I might reply 🙂.

## TODO:
- [ ] Create repo and add link to `chatterbox-service-go`
- [ ] Create repo and add link to `kyc-service-go`
- [ ] Create repo and add link to `chatterbox-react`
