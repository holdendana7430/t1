代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nwiuqymw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tllaeoug.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggnieldh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wwaxayzg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rgwblpro.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qmrhxyzh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3omslrnlb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3urarfjgr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pcngfjqs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ykylukmo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqtxnkv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3axpuqpda.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyahgojq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mxwkdgwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wlmyjiqq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3blofbzar.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sjjltvau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lxvcfyzf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lendctlg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gattsyif.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmppluc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3odhumhtz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sqjhhrjy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3stehjmqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuwewca.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3soyrirna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqmfdy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3boxbsuht.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jssfiden.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tkvkvtyz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3euylnefl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idlytezf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elpbncqa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bnidwjmm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ujbpjber.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrexosaj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mkkzjouk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3omdvznjp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rdfzkknt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wamwibfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jrokznia.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3znngzjyl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bvzjplej.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ntngdjci.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dakpkwbp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fkpiezmn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uawxjziy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qmgxwmub.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsuqodbi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gcxdrfwr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tevyfzil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ixlngnqd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nomcwumj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvfwocm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bpveushl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbfonrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vsfmokzu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3edwrsjby.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xwjbhhgp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkgayhcq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3phddupam.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lylqvapy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rwyzeihi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3endeeiky.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mhhanews.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbeewcvv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gozipeph.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3idnyoapt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jgxxmkzx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3idryewmc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tgqizjjd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xqbtoyqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3opdwihvg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pawclxpl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ngovpsnf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wycznztf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3aifzouot.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3walxorox.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsrlhddy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zpatyfeq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fowkxorh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ilekaqmq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yibbiyba.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hsczzkrx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhgeobwz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qcrfcfpl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekxelame.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ntwcgioz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ayftkxky.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emudkfmc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nchnbken.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ncwlacfg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sbzpcvpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dsoemvqk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bggkojsx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qvekjgat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fignaxej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zspreiyc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lphgwufe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvyjtbcq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tpcxikxp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fgmimgku.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvzhttqn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uivdhcec.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3miwxdbyp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rxoeyliw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dwmwqvpq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aasvwnmr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxoizegt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycktemga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pauocwmo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3etoidvol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akxmjcnq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jwtpxvqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ylbybruo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmtpzvq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nhkzjjwd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3iakkbsjk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pyjqfeua.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3avtbcbdh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hcyqvtnc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3stifmjse.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nrkobksz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tcfhhyjt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qbvvbfbz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zgbhlmxo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vnvfbexi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ghgwrdno.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxabjmgb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ajjegjbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jzohgobm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qxdwebgf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fdtcauhe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjrexs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lwcudrlr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xvtpkbso.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gufwzvtp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tojceksp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzktbctm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evdtnsse.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqhasfko.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3afkcyjxd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yxuwiwox.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwrnepnv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3euvswyzn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nmbrgcht.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecehbftt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xmndvdjz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnrrztzy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsjngpyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yicfqntn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkxnnpdd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crvsqldb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdzcqjow.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zpmovack.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vxzvbksr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3awclfctu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rljybxai.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lrhsssfv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxzcwruw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pkwbolts.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3txravlxv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pmrzjwql.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zyqvdwvk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ahwzntum.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qncnqimz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vaolvglx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ignadrbf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qzrcnbcn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ytmwzpmf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oikbdnow.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnttxfb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3poejrpnr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqltycgs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ofinmlvi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vdxqdhhw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3frsbotrd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3smjfvjpw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dkgknxbk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugjbzgpj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yvrrzsre.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xamoglyo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iixrcfad.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqlyanrb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsdbpfeq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmvwdfeu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bgdxyjrb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouurretn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svoonfwf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcjohgry.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dryubunj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvlnovlf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cvxyosir.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycjsnhgl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbkpyqhn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mevahevg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gonixvlt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpxgaobr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wdeahoms.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xebgdnwp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wliotonf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mxdftlyo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3elgsxqar.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3euthlpit.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rdemiaxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zasagalg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tfzcanru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ujwxqxlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beppawhi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ffkkijnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwgiypir.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qsbuqdpv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mkzggomm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pgeftlkc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iufdtcwo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3obmlmvcm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fabyklac.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3umpezhnx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3okjblnlh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bdojzrdo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftthskbx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3keqdnjkv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iykojwhi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gszmxzpm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drxcvceo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nrhaqfay.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ujeudvgn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzviqphv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbuvurv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mfhlbxxu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nsrcowdj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cnexqnzz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgztcuqd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xkjjwzfq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jufnigqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uaohrlso.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ggaapief.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3abgomggt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zdxdvecj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3klwsuemb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bikpyaba.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wmnfhncb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsitsqhj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmjurtdu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tohhlhea.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvdygsmm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qdojooyx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3prtbmkei.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hdsscbgn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oidgopzl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnekwqgn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhhejxvg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmfbasxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wxtnysjh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3glaqslbf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dxoxuroq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lefhrjxy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tosjcyms.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uwjarpkc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xwqsaarl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uqcjjgov.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgfpzkuw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uzxiknpv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3opdcuage.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wyevqsus.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rzlomwzt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3aiyjhwdn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sufwpfkq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxiktmvf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ghnoeyvx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gkkmwkxe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3myjonvst.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3szliygsj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3usspsymv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rmksvzlo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3aspawzbc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxlvfa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgjexahe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nmztsjks.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ojxznhbw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zcoguscj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkqnofop.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhamteqw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kbbbhyov.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gxrvoacc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmkjffdd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qvvnqvat.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbmzeife.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3atxgcepy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gudqgjdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hqsndmed.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osjzoyax.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dnzexwsv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3butmfkly.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dergnnut.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fgcsxbng.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3urllhwno.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ozlfblsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jockwvae.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jrqnraeu.html


<!-- 参考信息 -->