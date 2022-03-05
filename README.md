[![Test](https://github.com/snow-actions/git-config-user/actions/workflows/test.yml/badge.svg)](https://github.com/snow-actions/git-config-user/actions/workflows/test.yml)

# Git config user

Git config `user.name` and `user.email`.

## Usage

### Default

```yml
      - uses: snow-actions/git-config-user@v1.0.0
```

Default user is `github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>`.

This user shows ![github-actions](https://avatars.githubusercontent.com/in/15368?s=15&v=4) icon.

![image](https://user-images.githubusercontent.com/1297512/156898841-79f7a427-8e4c-4f36-9e78-c800d01887eb.png)

### Specify

```yml
      - uses: snow-actions/git-config-user@v1.0.0
        with:
          name: SnowCait
          email: SnowCait@example.com
```

See [action.yml](action.yml)
