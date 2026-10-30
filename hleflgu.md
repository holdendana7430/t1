代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gyehswnwz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gmbuckzte.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/ggucjeeoo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gpodkwrhz.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gfgdresck.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gvjmyicxy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gegcmnzkz.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gzstkakax.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/givwzhorq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gqkkoiazq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/glmqogzqe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwownhkpy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiemdgro.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gvhsiskmn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gxxngcnyc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grrjnqibu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/ghcnxeafq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gfzstwhfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gkdgkrqoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gkldwnpsh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gwucxmgnm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gezporeuo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gsxvothby.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gypjdshio.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gxzzmijmy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gyzyzkebf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/givspjzqf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/guzqitukw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gkokkdait.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gaqmvojwh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gljbwadsi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gorjzpvqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/guargtfjl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gismwizpb.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gqzystryw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gvomowymi.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/guknllnwa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gkvygyzab.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gtmqcrgrl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gqagzywqh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gydtakvzf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gbznytduv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gpcsjatzn.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/giuseuymz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwfcnwomt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gxoppdgcw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gvsfntrup.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gybrbdmee.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjkbzhgfv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gfzwycduk.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gtsdywxrw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gyasdtuiq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gpchyqkyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gbxedzins.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gveowdvph.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsdultex.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqkgszhcz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gcgguzsgt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjrpscvso.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gdkdzbxrz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gimyklqsv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gkuqyktyw.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gtnatumwp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gsbbcxuwc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gsnhlclzl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gfscyqxzj.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gzegygtbq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gkvsmrfqo.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gkfhfxblb.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/grcwcdnwf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/garixcmtk.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gveklmfev.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gbxxbntca.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gmplotujh.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gjsxmmbtq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gyxdqteii.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/guvturbsg.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gnwaqgruv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpumomarm.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/ghkdozwqw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gtutfyioy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gejqghkgp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gognxvmfd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gupvbnqmr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gduzgbojb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gvwdsjmdg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvpuiudyi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gadsugwoo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gxqqaxrxd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gzfvbokry.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtjcaczeg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gyitcfujl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gfhzsfqms.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gxzbavamh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gmtlwlbzr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gjocvshuw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gahvaurcd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gonncbbug.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gsedgglzv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpfynqpug.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gtcxhlqqy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gcllbjplz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtspgsbrv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/glapbhodq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtfyeznma.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glayxwpbd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gjnbfkkak.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gippjhyvz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsflbgqzz.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/glwptslyl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gcqnrpjwx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gelixtzdm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gxudunkng.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gqzanmrgs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ghycpviot.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gecivyxtq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gcziqlogk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/glpfkvrwh.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gndrqtgfe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gmhanicld.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gwvtkbmpd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqkqtwqbl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gnyvlyawc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gahqlhual.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gtdbmdbeo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gsvdgcgnn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gdiewjlfi.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/guwikyefx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/glhdrkibr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/godbtbhga.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdozojfno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnimjqmlu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhdlanub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gceryvgde.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/glalbvlvx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gjbqlpiju.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/genmcduqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gxyvwleld.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guszkrfpx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gebzwgiiu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpvbtirpd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmwgnyvls.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gvdspyptm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gieqysegw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gierweymw.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gmfcnieoa.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnpilfcoo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gznjrskif.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfilmrnyd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxqseueic.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdxzwjved.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwtbaeaaf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glqrgbjqd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/glxhqtalr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gfroaujxk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gafjlsvhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gwjasqiwf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gqltolhjc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gbqnjkswj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gdtjcvapp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gkgtditcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/glwrrfhyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gdmiiqghm.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gcrrrsgus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gvcvwtbtd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/ghczkffvx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gpzscsgoi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ghkfznfuq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ghsaiaprw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/ghtqkwwjk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqxqzttmr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gxqirumqq.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gqqjrwifs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grucgpetv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsjzafeyb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gvinhtpnz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvfjbkupm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gibvpnfof.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gulqpypgo.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjeyxlr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/ghgsetsqq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gzkprtfea.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqlsieioc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmsokflwl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gclyarynj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnmmbyxya.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gqqnsgvjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gljzgubha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gisnwaxbw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/graxklhxp.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gchmgtkdr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grbchrllk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjvruvvbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxbaeraie.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gujkvrurr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gkccwyiwh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gakpvqtsl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtgatfker.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/ggoutidas.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gfltmtpyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gphvtrxtp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gfwwuxoob.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gbpcawkvz.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/ggsqmrfcb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gqooqlwoo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gzaeakbvv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/ghguknbvy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gdwitvwps.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghureuxbo.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/ghyyrmqiw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkgdezwyd.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gsltxnojx.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gjhsezsiz.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/glooxsudg.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcbohtekl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghddebghj.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gkcyzrqrs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gwlnnhyvs.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gejhsnzmq.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfbezyvht.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gyvgvnofz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gdltcctqr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gtbugmtmn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gwoneidnt.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/giszyeutg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gbseoroda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ghfqqeuvs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gimywzcsd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gbqzxcqwk.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gtbyfemjd.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gaewviqdk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/goukculaa.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbzrlyeou.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggojndbif.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gbefdovil.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gyhddiziv.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqhiketct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdvelfszr.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gnoqpusid.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/givzlzgtt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gywxwbrsm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghmowxnwq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxegxix.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gadvftbit.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcroapohp.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gpjqbalna.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gzlhywhbk.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gssuhzqld.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gentgftzv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gizkewwha.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvlfsgyfp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghkcnlbmf.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpiazbbut.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/giuaafhkj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmywtyayw.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gcpztsdro.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/guiymbhrs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gvgiqmnvv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gblywlgzr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtzdqgocw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gzavdogmq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwjlclpic.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gkyvlwvhw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/guixttvda.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gmsqopseg.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gbrlakiqt.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/guxbifwke.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gftlabkud.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/greqbqbez.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggfacdaga.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtaeffwxx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gyyszmvzc.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gmdcgifbm.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gbxyxelfb.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gwpxxzqha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gbjqfukbz.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gmekeffpg.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/glwygzyoj.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gooahsxcu.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gfoxwzhwn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gyxpwmgum.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gxhgsddwx.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gaxwnuala.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/getgubcvs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gllwymvps.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gczpmotnc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvumknb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/govprkalw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gcgvyyqwf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ghvogpvdx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gheixlzfq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gxjzcfwss.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gnbmkskdy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glgdfeduh.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzmmcxvft.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gmtjgwukh.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glllibjpm.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gwnhztumf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gvsboxtap.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gshqluekk.sHtML


<!-- 参考信息 -->