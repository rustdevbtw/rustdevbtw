```rs
use bio::prelude::*;

#[Bio]
pub struct rustdevbtw;

#[Bio]
impl rustdevbtw {
    #[field("My Name")]
    pub fn name() -> &'static str {
        "Rajdeep Malakar"
    }

    #[field("About me")]
    pub fn about() -> &'static str {
        "Hey, I'm a Rust Developer, who loves Open-Source!"
    }

    #[field("Favourite Languages")]
    pub fn fav_langs() -> Vec<&'static str> {
        vec![
            "Rust",
            "JavaScript",
            "Go",
            "C",
            "C++",
            "Zig",
            "OCaml"
        ]
    }

    #[field("Contact")]
    pub fn contact() -> &'static str {
        format!{
            "E-Mail: {}
             Discord (Username): {}
             X (formerly Twitter): {}",
             "rajdeepm.dev@gmail.com",
             "@__rajdeep__",
             "@___rajdeep"
        }
    }

    #[field("My current project(s)")]
    pub fn current_project() -> Vec<&'static str> {
        vec![
            "ShareImage <github.com/repgrahic/si-rs>"
        ]
    }

    #[field("os", i use arch, btw)]
    pub fn os() -> &'static str {
        "Arch Linux x86_64 with Hyprland (Wayland)"
    }
}
```
