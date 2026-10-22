代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ucwdrhts.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2epdyvrja.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mdgstwot.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrnjgtu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wxkocylc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2edsasfbc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpdrdflm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2acyusgmr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2avyltidp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2llymgval.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nyuudtmy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2permyvyr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nabtvoza.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ieigbjcx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2okwryklt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tadqlxkb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cijhclma.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyyzjrdt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbjotsz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xlmsyeip.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2exbsydws.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2oesgmwdg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2liziafox.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2unjcqzud.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lgsjlpuh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvxgyoz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kthenova.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jfbumqbr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrdlemq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qvdbcllb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vbvtfqeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2omkfpwoj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knvehmyl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ovidtnuq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ecbpflbg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wqdlkvxo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjqkrf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjrimfi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2buxmxjmc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zrvwzuvg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kewstcdj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2npxeasyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lbybzqct.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eqfaneyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hfikkdkb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qvhvbnfj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lgqzohhj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rfsxbwmw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ixdoqvmr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mgdariow.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrtyrxn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2glbvexvl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2knvkqguu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvrmucjp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uzkaswmp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jrjlkrmr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ieswriuu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jqtvtuww.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdanexn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tcvhurms.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lkhqnpyt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zuovcvnn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wbdifdvc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sanxnoep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpuzooas.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nhpssmln.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vnjinupp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mshilzrx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2atbeufcy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbvqvwy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqtddooo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obexacra.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ifmmsyfw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qokvgtaf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uyhnxacu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mfxnwmcs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lxkuvyaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qxyfqbal.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jvidqajl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiwxyufx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxsmzoyb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cuyppyuf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyscssun.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jkjcvuza.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qwchgwtf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2spwxzuct.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mkjtgygp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghitpyyk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fwwhzcxr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qbqrszyx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cqqesgms.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdxattem.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2taxjpaqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lfrxazme.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gjhxnfro.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkwrlfbj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xogkhjru.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ieyswchj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tuhkyrce.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dfwloaqr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vnxadzef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdzgxeal.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eoewmgya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlnafatv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hbnfobwm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bxtvrezo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbehtetp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dthfmppz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nrclomsg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pekysfxo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tgjxoyuq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahfqwxfa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vguytrag.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2aeisgaex.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2muhczqhb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jrsfcawx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2thfjpdci.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yhjzvgek.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjhlck.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2blaruinq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvuphpu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jamjsxvp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xsunyofm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kqkhdkxg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vpcixcxf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2acndfnjn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dclfcbpc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ybvodhex.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qhjbaoph.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xcapteyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mtjrywau.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2svvllvaz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkthxip.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lpdychsd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ajiodvmv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xwsltcca.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gjzgwczc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aholrbmm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2oflqrfvk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gnkwkwkt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pfzuikzd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2njmdzaue.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mebhoixd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apdovkkn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzuorhhx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xswfafkb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ixgusbwy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwvyulmg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixtmlino.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2anwdvnvp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptepwsae.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzrpssty.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlpveso.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqqkuztf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lshplyum.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvfhtqee.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgkvkkqh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkfboxnm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2npaifnuc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gatqrmqs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wlzlnpls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bvvozphb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jpcildcj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kblmlyxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ieczhpuo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gobtsoeb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zcfiijoi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nesaxuyq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yuottujw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gvgjwmqw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zcvoknnp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yhhpfkkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2airgxgye.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqhblzpf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kcnyzbbm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2plmtbjmb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nyhymegy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eddmntmj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kspwwisv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pqcaixtq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpfawr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2poswjemo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ckeawkca.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llmonrju.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bbxsomtk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sojfaalg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dswkbekn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fwmagdeo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmhwdmrs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnprzlhj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ripzyyql.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uouuyvpy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkdtynje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlkwulgr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtghfcdz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dexyaoat.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2omgachas.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ragzslbq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbxmdgrd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vuapwedu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2msygdyaw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsjdbhdj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iskgfrli.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rrdsztmi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mxdioynw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lmsvvdlm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mrrnlnkq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gparmdjm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rlkqucap.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gdnpjxgx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rbydvprk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pxyjiwwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsbfojtl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hynxajnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbrnmriv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kbffryag.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2szngcqfe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpsjksju.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkqwyyzh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2inuthzyt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyfaqjbc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dyhcbnaw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ylvfmqmn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uljufido.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2somjfikn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rsgmmlhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibwbkfam.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmqywud.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hnfckbcy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qenlyiec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2coxriltv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qnomumpa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2slitbiju.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hvkkyhwt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ygbbrtwd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tsjauunf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tfdtzmlz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2shwshzmh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lkhpndty.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qnyrgrvt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ikepajlh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ggtgvidf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tawskjww.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hyqblpjk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abihdnqc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sjvrvabg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ipdztevq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lptdugqr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lhdiueau.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cbwolzmn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lepoyplo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2znssgxkx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dnswwhhi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qxmzadjw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gvjclvka.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuzoopzf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rhvrvmhb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqyfoe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qihkhwml.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxngvjvj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gjnvrifb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wasffdin.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2amjfboxn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imuosicj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hcftvwrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkmqbqbe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gjmgypma.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxwlknsn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ezghynlo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ngbpcojp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hliwftau.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fikqowcj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zpnsxjhk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zczxndac.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lfhdexvy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2svqyibfi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ycoehvnm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zohwcgsc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hambrmiu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oytuekta.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2orejoycu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vgajsujh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyftqtbc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzzgynxv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ykspqcfj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccvrcepa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hiicnzkj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ozqrpfhd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gjjbttgp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhsjjovs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gincdoyt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rkcegwlk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epthhtzo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hzirtdoc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2aiagkdbp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkztwju.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iqvzoura.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vxnnhzkx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vovdypcg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ljmxklfr.html


<!-- 参考信息 -->