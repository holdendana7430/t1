代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qwbwqreo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gsvlkict.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mqjqsxgq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtlejf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clibyvvq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxsyubt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qmwuwhjb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xqhaueoa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pafycntr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3arpyrbcm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3upmnpfij.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ffceapor.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kgxzejas.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rldgmnfz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mxccqoff.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3swpncjmw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sskweapb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3knujahfq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ejloxugf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nivhpvas.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vyzfkaly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xflkejrd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sdsqvimr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fefptixj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3senfyogl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mfjtfxeh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3drjrydyp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwuwmgp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uibrckvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xqcvldni.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3agbgktpc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yaardikp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3afvzamgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fncberzr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wmhkrhuj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vghgqwjg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cbfxcion.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3kaheptlq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmguscs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3eunoieui.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3aydhzyom.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3spvfavcq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vbdozgha.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3onkochge.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urgphjsr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ustizrwk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kqcqdjui.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3cygycjos.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aacgsial.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rucejzxw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3atuqxfzi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3miwagbea.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hrdddemq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fgozmqbg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3igehuwol.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qdjrbqoq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ghllzggs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aafqamek.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3touusbye.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onqrehhs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ezrsdaut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uolldnpe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jfmuquwo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3imtebels.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ozimtwbk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yiumrfzr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3knlnngja.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tqauxjxc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vtxtnkmq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3orffhiyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbhdyfwh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwjyvpbe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqqtodch.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eiukbggf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tjhgacej.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ggwphcsm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcghxlh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dovdspmw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qqqjfcxn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ylqhktpr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3sotedetg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hsoalbhq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rrxalkjw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pgcxpbfb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cwrbrrsq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lpaerbld.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bbenited.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gasiozmi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vahucjyo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wjnautop.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pjejrakz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mjftzvub.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wvksrgki.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qlmwovgw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oigxklri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jvddvtjh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qixgxipz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uachpdah.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cwgqcpev.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ieclbxxr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zyhoxblg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhsxshpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aaqyasvl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wdlubtmr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mptqfjaq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3einhqcsy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tqwxebva.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yjriiwdg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cstmbqrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpuuiaoz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kqlltpnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgtgjmsa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jfztvpra.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gmcvdgik.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vgefdvni.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hrjvpygl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3faqoyxjq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3irydnqce.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nlpmgbyu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsaflfcl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahiywszm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wngjzjle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tvttvrqg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmyjvqgz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jidtnsdh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hsavjuad.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iggqxorj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rqzksltk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3morfzgiu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yrnvorcv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ixyggorh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mqewwqkt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3juovutyx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ykmudlyz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vdtewlco.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3irpmkgdl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ijlejrnm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dwcasbtu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3alhmnljq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3musipjzr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qwkoodrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3shzihoif.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jxggxbgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jcngwmai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3egeoltwb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovcfscoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjiwvro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jofmeein.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eycafwki.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bjgzuxub.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ussejdfo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwfxyaip.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shgoabqb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uzidllkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rkwcuwrw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hloysvpg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3islrdvbc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hdguxxcq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sccpacvm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tadmzkae.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zttezmnn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mimpkrvi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jpxcoutn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hiubcdob.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqxfpyom.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tkgqyaoz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rsatopah.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eelaiylg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mrkkrsxo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tvwnoacd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dymwhdse.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cxjptmzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vkycoxtu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3olgxtytw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xtmntais.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3sqweyvpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3stxrwktk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtruffog.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tpisobns.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhrpdifh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3smalmeem.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ummuysjd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3addqjeeo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oshjqpbh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tpbejldb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbiywujw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdtssrxe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iynvdpxj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hatvkutr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3danhccrg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rtvneqks.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtbazuxn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mhinzaix.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gikjoaia.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybayonva.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3igexjowi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwpyuxiu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyywlmrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3frptzkoq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmrpyhco.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvwzdzsi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eriqgvgb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvrcbjps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hiqspxpk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3neeusior.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aimfufhs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlyxrekd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qstinfcw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dbnvqwgt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ucysfiaj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qmcfzpeg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ruzkpozr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3prwlbxuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rawsalai.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zykfcvav.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qlkkogpf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3idfotdjy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dqvbguxj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vwnnqwnn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3oqwviwve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfspntxu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fiyirsui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpusmjak.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hweddgux.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zgqbivxe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofczmhyh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3juhgzwcy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3aqwrnins.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcnwqpbc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uvxxcizc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebvpvquv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiwxzfrg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3prjhcbya.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gvakeusm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upljjvcq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3owrcqqie.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iqroowjh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mrxtcsxy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qyqnihie.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uosvsrdb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rrmzsaqo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3elnycvzt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oissathu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rkytzsyb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rtnqapxz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qiilvzzn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eptgaled.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xruiqfyh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nirnamgd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yokcbduk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mexurcqv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nubtbsfu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trgekuuy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3izsovmid.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3onaqbmgw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljvpcdry.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tmnkbwzw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ywjipqpf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtircc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3efusxoxg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vglafdmk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mibmcymd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jumvdzvs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3msdwfxtn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkrrdhai.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bpsitfog.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxprhocg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cgtsezix.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kosnyjdr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rpbcukmt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vsvvkfsl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cziitcgp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3weomfkfp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uzvttbva.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xcfclkae.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hczimkhk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tymzcxzq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uygagfnd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gzmpepme.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hwqaifln.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gcgubmdt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wdqqmsib.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gimptdae.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nuruzsir.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dohtlxnu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xujtxbua.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vygqxodf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qffxmvnh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zkgnobql.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3uryjppme.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvunnvbv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lamzluee.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cibsyamg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttnoorcu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xlxhsxyd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bajgltee.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3thojstzb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sidvdbmi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mbxcslfa.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ebamxeoi.html


<!-- 参考信息 -->