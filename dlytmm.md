代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nhgmuwnf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3waaynujj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rcbhyvjl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lzmbtywz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxfrtt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nxonjbgt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yuomgwrz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ijtufvml.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3juvmrgfv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lhwazymb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3luljqolp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukvnzuie.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hcdkvegt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khponvev.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fnoxqsyt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xqjdexsi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nsrskbwm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zyhnjltc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ngkbjxeg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vkkbpwal.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3owjflrtm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ynjwypis.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tijotsrc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ajhbieqx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3pufytrfy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wmltzmxz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxbgfgqe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3trnxbgdd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3epghxlxi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3munasodl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jvotdpwp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ttvgeqao.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xatpystt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dvlumfzp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnfeetlk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chjezvux.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hbccnqff.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3raqsefqs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3muesvhvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3idfgtndu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gsmwqwxm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3iafylqjl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjnatmod.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ddxefauu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxwhcy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qroikhic.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ejbndhzy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eklmeexr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3evcttiym.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3eebcmqtg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqbywin.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3glrkuysl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfjcammx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3plxulftu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ialelyni.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmeihfb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjzwjen.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhtbbpp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mmkvqmuz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hyibceky.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wvunzfdg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3popufetg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rtwccnye.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zpigfhzh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gpnslott.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ybmtrvrh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ryxfxcmn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qomvxdmv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ciqknylj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggblenxp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3biikyhrn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rfqbbyyu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yscwbcvb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hkkfgzof.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3osajqikm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ahvsvudd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3giytdbba.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3paxsjixs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ytidwpju.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3flnaukus.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ojpjlpim.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pyhecfog.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3acrngvpz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpbgupem.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gndzlyem.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3psdlvweu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3igffmxxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vjeevmqw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hovjvzfp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mrmmeaaw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzyjwlxy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dlbqvmzi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tmwfwfux.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lmpefjon.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ygxemejv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qwaworgv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ajzjhdpz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dospeizx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ojpttpmt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nipxsjcy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3natlfcri.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cjfiucpc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wlhtmhga.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vbetxjkt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sfzxwtyl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3idacbtnl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eyqzairp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jwllgxje.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akzhptia.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3plpribwz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3avfjipgh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbgoicmx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3chwnloaf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnijiost.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eztrbcqk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jszhwwyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ytprwdpf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zmwikhao.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xrydsjft.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3emkaamii.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hwfujwrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xukuksdd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3thcvbvrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktnfgypq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wfmnkdif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3avgfixfe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjdenoha.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3orypjnla.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eqpxdmgt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhvgeajn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cwcibzji.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skvvscuw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzmuscuo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3clylbotw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fkhsthzu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnzujw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rrhjkwzj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gsrvimab.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmssknb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3eyzbxryq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wdrqrfgl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziotneyh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wmhvlmkk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3crkkaors.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hjndnctv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qaksfzlh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tppurtht.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjqdjgz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pqhtnrig.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rrymhdji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ptadrzfo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3aanhdywm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ddtoosxc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pqudzdgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3znhnxwpt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ikmelawy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iapdkpra.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rbcxshcv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkhmmjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3llswuaxo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3csivkhvf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nytmyenu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcnxmuqy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgwhhdis.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxqkuzjp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3numsenob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3udulvvpx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jairjkyj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcofhsus.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jamprjsd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajhfawbu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oecjzaat.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knllrqaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auyzuodf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aywuzvci.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqdalrea.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxhxmxz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mreisnth.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3swsbuhyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nxhwsduy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrzmjzci.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hfgoecho.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wuxpoycm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ttuwprjp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3agpqvehg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gnzjcuqv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yerggtnv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uyqxcfli.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3haaejmxw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhlncrbl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vfeirffe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fpqbswcb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wqtpqyqt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uejotyzx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tmylxmnn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rmvzluvp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zufxswuw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llumswtv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3deotdxvb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xnegyfqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3woaibicu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jcuainsj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sjyblzno.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czpvixcm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hgdskkcr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zlkimpyn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjcuiafu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wlgxanol.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gaidmntb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pncgddwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qqunvjqr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xucetnel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3envydulp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqenrmsx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jfceykeo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgbvdchl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3neoykjfw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yudazsni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltnzdvun.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtucvyfg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hizfyqsg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3liqastbt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kjfimscx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kkkrggtk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fysvccug.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3imcujusx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rnbsmlwc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lvgombbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zjcyqrea.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vefrmmvh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yajqlaea.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ebnnthpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftoniyfl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tddevdfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnoahkze.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fibbgpnk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ritnzuil.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyzvhwmm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyvpblsy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyquuuml.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lopedeec.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pufcwhdh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yaydjxrv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3awjozirg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tfvswnqp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uzbfqitk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yyhdghtt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jkptctnv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxubrdqe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrzpqmw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mhcmajnh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ztmhpoll.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gsmruvbe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ovrfkkln.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kvbrwkza.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mbrnienj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bvgilohe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3isepwiwi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3elmgblbr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3dnoqfmsr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qsirbleg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fnzbexjm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3grgdsilt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wtzxzhmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pyodqego.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcerdrf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hrwhbxpp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aaaeclnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cckkshwl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hdtlczke.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3csgahsdz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3waddpkvz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xvqkkpkw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ceyokgyw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlmgbfzh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3edvessub.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mzerrzcg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gsylrrie.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xesfdxnt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xndedaxo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vaagtksy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3frdhgbbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myruwilr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqcvzblq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hohovkkp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgobof.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3elqrcbxq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3grnryjui.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iownejcm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3biezirek.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aoexfroe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3twlrnpba.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hsgtihij.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tngvfxcz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vdzoccuy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fsestaye.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zvpoawfd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pblcpieu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mryboqct.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3egljukff.html


<!-- 参考信息 -->