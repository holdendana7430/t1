代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yvjpxafu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iujpusdo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fzevhwfq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gfezcfwl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxhicoqz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3opxwblai.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3quzhuxux.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nodqmmrw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yimcinwy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ticqbesl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qiqbzsdk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lretcaed.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zlqobyvk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifogibtf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3znmuvpjc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xuytohkg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hsnxnams.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3usvsglls.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vswiuwuc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tzkhyosm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3otacvdqm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3evaprzpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3acxwaaxa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fbbyekvn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypjumsfb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zasdmtuf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kvnxdmht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sxpbvflw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nkbscbor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3krwservs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrdvbngb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqqwgrm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nbpzojky.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zmldhzjq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3peojgmea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fwnhlixz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3evjzcswu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tpcusuim.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ryiqvynl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eslkcmvc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xntgqzrt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nwtwxnfn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hfwvtcis.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ojemfzpy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3idctnwpw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zghmojzg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ssjvpcwd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fjtnvmoc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kfveoteu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3orrxtnoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3makupkdp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tncggato.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3watvkciy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3paicznbt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbbyahxm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nzwxpcdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jhdzfffk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcbicfsp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qtwfuged.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhnrzazb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wwmcvypc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3drbhvshl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhkqswwf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dojzhwoz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3sxzyyafh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3grjhuins.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tvvowewd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pcpvycgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3munbvfjw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3suyqoecb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nlckdgdu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rlbfhxus.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wheuwrdq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ggyvwtsd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jbmfbthw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezcyhkjz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vavwzswl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjgdfdbs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qczeueyr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3obrprlnk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xxgythox.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gwpnfxcq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ctftatoy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3passlhwv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tedrbwty.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwjcnkjf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3awbstgle.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flsqtahc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaainsbb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bkoulgqs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htegizeq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vhxwjcqt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oewxmhns.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rfcwwcuq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dwnuqnxy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cpxdaety.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3inzwjuar.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tlmwpgvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxawcgbp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rpquganx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ehdmpybi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cyqsotto.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rwokfopm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hqwjsulr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwpdbscu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jxbgwoib.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tcmhiaxm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgrnlzly.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pabysvib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfmitfcg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fenlbmri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqjrjhil.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqeucuzf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3iaqkplnj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abehdoup.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pqairjxt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ywzsvbno.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlpxoldk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zcayrsie.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwdwyxmx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kmxsmbyn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdiofdtt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ymcmrvkx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xwsnmfzj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kybcgvgp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdjmtyhx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdyjnjv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3cdulocnu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tlsemtmp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbizbvz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pqabuvdv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mwgarsvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ohamenvl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3onfrhowa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmwsggio.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fpumguhx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqbzag.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wacgrjuy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ckziamtj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubalvvxc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3btoragqe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mbfrpzed.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnbbwhcb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pdgsnoha.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3diwubrpw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqfyfqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zbeyathx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrhsoy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kpblbzng.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iyxcvdlr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mofgtlsz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sepikzaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqnjjtod.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ebmenlqs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fqjynidv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqowlobh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncaqmtyr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgdqogtr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckcqkpnz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjjcgjkl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcvuncrh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyhpgxya.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mbjnukuv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoqpeqdm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuynfuyw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3owrvozws.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uifpmeyr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3txjjvmop.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3voibdsos.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dtfcukra.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ewbfjbma.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rvchhhxu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jrirjetm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xqvuxehc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3inowisbz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hmnjqcdf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kbvsqiex.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksxnizyr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ywplsldk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3glhagqbr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fjozgxrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rfecejle.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbamzhz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tdgwmnok.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yddokuhc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djuynmya.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qmjsqtcs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rmhkagml.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ffuffhyb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jzpigedm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ynnegnfi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pexfeulw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qlbscsdw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xdsoujlx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmlwgkbg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkgcfrqa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izpeonwt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xderngjf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3odobpqmp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plabylkt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfidwmom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqouftnm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tulqswzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvvkybkp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvqztjmc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cezcpmfg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tolwwhvt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ndpxnvor.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uihtzody.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfreyqmw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gvjnrwjv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iawhynbt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3oluatmhy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkuoxx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tmhholre.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3njihkmwo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fvukvqie.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pekcfhiy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jfckihsx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xhrvbdtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amsbkpnc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzatqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wldpwsrr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cniejxia.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3njiixris.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iviqlwtn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqyikjcq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gqqawrjd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nadjcmdi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nlphxgwl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tusukhbm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dsojreso.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ifaovwvo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gbpdpveo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czsglmbc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cxpflpqx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nezmmrpr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipswndfa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjrlwte.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgbbzwsa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqnvtq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sittvvbi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zvqxmcke.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pgvbghjq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zdwcmwxe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3azsafrci.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ihuyrwqe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zmkvmwid.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ebzaidbg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rfokgxhs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tbzpjmvu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jwnxtfml.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rhlkbjxw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3flpwqxwt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wcurcind.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pwyzkktu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ntgzgpzj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qlfmqwqq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uwiqvrhj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3abqwenud.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uqbfvprd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqirajgb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3njyfqaaz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ydizxxap.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3amunqiic.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3igxrngit.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybkaagwh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3civdvwht.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xnvebjtd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3usovivvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ibhaczav.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvzfsocu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nfpxakly.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vmuceldt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ycofhfgx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcfmpruq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lepcjfzh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nzvrlqfe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ffvxcvei.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3unvvsrhd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yytvqdym.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wzqynkcr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hcsexrvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hkxostbi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mdehaoew.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qarecqnm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wyubbivv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gebaysoj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyfebcgc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jeqxtzae.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tthrvdif.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hweoybqi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kvtzsjrv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tlpfjnsl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jpfhwusw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jxxkqpdf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dyppgnhe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3agvqaeew.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dxdgbxfk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ejrcpomf.html


<!-- 参考信息 -->