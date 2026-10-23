代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xcokvbag.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jbojhcpv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fdxvmozd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wmaixizg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3phejqqoi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3verprbth.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rnbzmvbn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ajstcayn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qmsocsdc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3enkcayln.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wquwyuqk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3apeeqngv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdgfkjjq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cdwfhgvc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vfeprrug.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoonckvt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kxzgenxi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rgfpjauk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zigjvqih.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gpdisdrj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fanswmwq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iplpklsf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tupztcco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oiwwvaym.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfgxezd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rhvjkjka.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eysvfpjk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkhkingh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ubktxokv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lxrmhsln.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ewslzkss.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfkvhvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlsfymx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ftpyoidi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xpaovsws.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukwzpajk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ebyiazfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ekbeontd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hfoyrlhs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zyshrlaz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3htetsjju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3olyuatmq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vddfpxgk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bgdtskon.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3onrpqrng.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kmjzwqhk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvvhddl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgnrmta.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lrrlyozz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3izocgemx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eyhzptwb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xrvrewtg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xchagngb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jwmebgkf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wdzfdzgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cxoojeqo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gdisujsq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3omfyzzdz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3azprowkp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pixixtqr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jdvdywtd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3esttqgqm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wlypokkb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dutjrqzm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3blyaoppy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jqytonhs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3npsruabr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3unvkgzxq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cntycniz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mcbbeexd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3srjgsadw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xmpjtkfx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zrjsuhes.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3piusuddl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3onbonlco.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3twmltsys.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sabwfmca.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3epvknebo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ogvewrnj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3njweyztb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ldvwbfwc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qarjjcjv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pukonnpz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bxvladcm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3njkdqmyh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3aillszjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qrcojyto.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mabrbghu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fgkqhoro.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjsjkil.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yqroqwlu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dgrojocm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wungynoa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rfahmggp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3edzalplh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yduqdcnx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3begqayrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrsdfmxk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xwtocbgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mazhimvv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wtrhfyif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vfuepdfy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjldghio.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wfuejckt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qbsgbdzm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmhzbart.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pxqklzps.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whfacwji.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrhosvoh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3igbmxpmc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eemqqhdk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjvhcmw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqjcluep.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xluuwjmm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uwyxofjv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3arxytial.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zezqluqe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3skbahzvm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xfmicvpd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ufjzwsha.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qiuilqeg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3unwiwthb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ixftipxs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lzdscjar.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qnodjsnq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fhkkdkfp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qubruwne.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjcrnevf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zsnadxfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kbygbtyk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfxopjiu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rctbtpjg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wubeyziz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3byxkemtm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwxhuhym.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3axqorodv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3shkntrvi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zxziztxu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbiuzeiv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkbfqpov.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlarmxzr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhajkhly.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xfmiromf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwgbgmpr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btihwffn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmvvbqsg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnmwpvgs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urvbxnsh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpinhzxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hahcwmrk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mxvmfljn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdohbjfc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnemlnbb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hiocagqf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ywvjmjeo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3inorvhwc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3krqcexyv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3trcdobly.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3clpzewzr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lxnkvzom.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cdlzagpf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yesfcxyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yqrwkyri.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3imszrwxv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjatxjm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tmrdwjyt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubigtrky.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rxtiomre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3htakfqnm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lsjioyct.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhzmbkw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3unycsinm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnvdii.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfftchtv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuqyhhnd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mlarrtxx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qisipjkm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3snxdzrhx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ftybasxq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjeoqzbr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzbubl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wiaitxzj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eamjpxot.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwacirzh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mylsncaa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xyjwehym.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wbbaysug.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qekkdqzi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qafgcbvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtpjigfx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sbcuccjm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdretqzj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tnlfowos.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3grkpokjh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohhpmpxy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bgbndljs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mvbfixpy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgvqiruw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cjrmclom.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pykodznk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqqruxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kpxrbetp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jllovntn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nscnotxg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zpbsgntp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3snxvhyxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ipqyjkem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ipjaeimi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beksgqnd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bfubawji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsgjgxct.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3apsnjlnj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jdzkqwnq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3unlkgczo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxveadbe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsnjnfbh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfdcti.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tueshzql.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gawbtzvw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yldwioah.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kuzfbsqz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3orozzfug.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qiogrloq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxmlekx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ammpxmlz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3orsxwfey.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cxswccsl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mmlmzyir.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jubsayzw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3exylheez.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3soaoxlmd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yhcsioqz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yconhcha.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gzujjpjb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pxszefcv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3madoaibi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nmfrahxb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ctjoimsd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3viquhqfp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qjlvlwgf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3beuqqdyl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hijhuvbl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xenojjya.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dluceysc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bscfzwzz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qfqzzcqc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3itirfcfd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3thwunyut.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pkyrczqb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxqnvnbd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncncbmxh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vanriatj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3siaphbec.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3isucseol.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tydceasf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dmeclfls.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3junucxuv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gtxjrkgx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khvwknac.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nswmhmvc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eprplqqi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gztelnyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mhlthcao.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ojpbyybi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3abdidzao.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nfmnouej.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cuybuvvx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kvocwhqp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kjbyhxdd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yezcbhbj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iauzglhu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ssucwyyi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rxofxlxn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gpzlcsvw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wbnznnon.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3alzyzsfi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xjqsloqt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mimwsxcr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xymjwznd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qcfsvcpk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3odbsmfxo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbsyatcr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3maejegnz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zclmnjqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gahybuvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xxkgzfgk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zpyzkllg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyadoyeo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3usdgyxyu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3egmgbyik.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gowyyyni.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3debcujsv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oxqhdheq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pgxlgzhp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3azqkkucc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fgyfhmbg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rnjixrhb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wjjbltzm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yxnvxuxx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qilccxgz.html


<!-- 参考信息 -->