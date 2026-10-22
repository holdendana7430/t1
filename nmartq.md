代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2imsibykj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ucexplmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2anyvfqhc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cnatalme.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gsgynfwv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvgwnkak.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hvkqmqzj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2flrklkpt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bvlefshn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zqhoqmbc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yjcihkdp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vnnlnssc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lbtownev.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jgdguqvh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2irupvufy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2syltusld.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xgbhtheh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wtgciist.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjafowpy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2avywukxp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lqffbpzf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mfohlkoy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fgdhfscb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vmifnkhi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jjzzlnyv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ashncosz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnzslsw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sinyvimv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbwyxynb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cskqlbek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iiutdbju.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxunyrwi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tnfvalka.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2knyzkgfc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqwbouo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hwltzwuk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmddjhp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2elptkpty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2catyjxml.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2htqfvtso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xujwfcbn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mvasxpwg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aaenoszw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kkovhbky.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iognjeji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jtqtroxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ouizjmel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpixhmgz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpzgakt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyuumrp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sjlxebrp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uqvkhwks.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ykfwurcv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mtccsnrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jaxnatnc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kgchokni.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2odqyteuy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2opcrwqxa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bjsnypws.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eynyuuzi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2thqakbrs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssgopgvl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrobslys.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hmbqxwdv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fxiztrlq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gerdhkxh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vbqibzom.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xcbogugo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nsqmkpzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jdmwlxbd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kkhbouyz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhilkob.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2izvxaklk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ygubtprq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qpmohhox.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qabhzkfv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2geyddrad.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2eipralzc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vrjdaqnu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jszrkkbg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vjtaobns.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gkgobjyg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iplsjhkm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xgdgzoco.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wwdnaklc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2asglgonu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bbytsfen.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jnyitpmt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qebkhjwr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhgwjqhm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uyexxrum.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zsgibchg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cuithdtw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zotnrpfv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mvvwpaux.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hdlrycpb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hdoxryrd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbfufgtm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2murcuchd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pemjlcsf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xmqrxieb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zhjacyku.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zofjwsqq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wyfhwiif.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2svjyvhld.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecyjikuc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2emxjiatk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2birasgdc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2imtkxpai.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pmtittma.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xgdqhrme.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ywqchmai.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qojhqvqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raotssyq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wrkznfbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pslorvlt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjvjhryy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lezuihll.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igpmxqux.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vajminxs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2umrvhthm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbqqfcrc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ulaqslur.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccqhilnn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sdbmpxfn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzavfujw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2aynwfsyx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2julgtlnm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewirwcpa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztheucbb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hvbmuijr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdikdwkt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2efbjiglt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmmvyrc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ajxughba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zaslmiri.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdjaaskv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ogrgadnz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qffaxxrq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgfbsrai.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lewlroka.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dfitwzom.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vgfreekv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2voqccmha.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2clgaimfk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2eiypgwjw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvkevynz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fuwttiea.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wusowjnh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hyehvoct.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cvjqmvor.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mlmprggc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xsowkvca.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nlsknpxt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pytziboy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjmjljte.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drzqnmac.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uglnirty.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rrkxanky.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zojtpkhd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcqlksfm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohzipnqm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imhmadtb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zxtgdutp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlouonqf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snbqlras.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lznnjdku.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hujystlx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abzbxwpp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qtifyspc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lfbvbgej.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xwlwzvhu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yrbbbpuk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gdqdjfso.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2thbhweoz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tzpykqnu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fggekkmf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2llvpbhqn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2shmcmimw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zkevafax.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kdqbafpo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zsvizstj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zpdtvgsy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fcqlnfak.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mfuwavck.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sedcjkmq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wpxszvwc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hngpphlg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wvdjpezo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qokqtlts.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgnubgec.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tezwbebw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qbhcmhnm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ysbiszie.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ljabdllb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2glulsvmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2oilofuum.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2psagvuao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvjxwkmk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dftoqzmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uuurbtig.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iirwjxax.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jhqoecbz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfmdfzlb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvmrpjbs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfbiwpan.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hspeiotn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dotpswss.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2furgbjrh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpbdpsaf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqtpnltn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2klqxtgsp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fhpxqrxe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcknvdkx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wtwrtilm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2phciywie.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qvyleuzi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pkeawgmn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cglnmyxj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lridgjfi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ajpuogvd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yniruogz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sllymize.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eyrhupst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vounzrcd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2rwycrsxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozdxfolg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fmmotygp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2npdkdeyu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kvjntbsn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2msjircfm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2smvzlfzb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jhjvbgiw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2paaoveud.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iclqlacq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2erdefgis.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpnthoqq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jtlqxbzw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2oklvdmrp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awniuiag.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nljjwhfa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdhqtup.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2oecxpjsm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2aigxudqe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgwtkpa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2paybeusl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ulczgmyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wsecrxqs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2obpggdwx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qjpckuez.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ijnyqyti.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wypluhps.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ttmezvww.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fhklavby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qnbdjock.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cijsfwdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdmqcyb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nulzkdmk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2taaaaqwg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkpkzauv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2plzstlsk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzpkdgdx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hfbcthnz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tnpkjazv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2txashslw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufgujfka.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2azraoaxh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjsdgtep.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogwgsesv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jhqoorme.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ofrtbemp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzzzrkpf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2inkafjqn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2txnobneq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2siiyrtco.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aacmqdvn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bnekvjvg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlfmbbux.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2viwtiiit.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rxwcxpqn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qwvdjamj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mbirphfj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fnzslakr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qrkshqfx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2knqcnaja.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wpqafdrq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rlxtmlyh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wjmqxhdx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2towdilfl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zdvbjimb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jgpluidb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dswolmip.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2egbthapt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyspbwck.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xybrukrd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdlosqkc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gnrdwtqn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2daopgpeb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cqbmjtqg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wcjeqyjb.html


<!-- 参考信息 -->