The image used for generation is [namely/protoc-all](https://github.com/namely/docker-protoc/), but is called directly "protoc" command or using https://github.com/timostamm/protobuf-ts for the grpc-web.

# How to use for dev
1. Open The folder in vscode
2. Using remote container extension, select reopen in container
3. Develop
4. Run "gen" task
5. Manually manually replace the gen files of snoozehub-frontend and snoozehub-backend with the newest version

# Notes for who has to implement them
- The comments aside some fields are assumptions, if a field doesn't follow its assumption, the rpc isn't valid, and should gives an error
- In proto3 is not assumed that "normal" field are mondadory, so you have to check if the field exist before use it, If a field is actually optional only if it's explicitly "optional".

# Improvement proposals:
- Possibility to modify an account
- Get a list of all my beds's bookings
