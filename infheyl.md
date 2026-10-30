代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gsgdqboge.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gdtijgzzj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gqnvcdzkz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grnxytibs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gobpdncww.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gztwwreec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcngfkvnd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggyuncyfy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/glvipzkzf.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqleeybvq.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gohzckrcc.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gfwmqnycr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvijigngf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gstapmwhl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gteujjeeb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmidxjevz.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gbovmkplr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gflojhorx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/goethcait.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gcxdnezfl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gzkkvijum.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gyyyxsmnz.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gknitdovv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gzurfisbj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gpneqxxud.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gxdumzohh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gqvmmjjbb.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gpclsseix.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gnicfyoma.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gxafdgxas.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ghzpvrxgz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/geacqobbm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkbljrdum.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gxaqtfyhu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gxkwbffhw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxrfdpcpw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gnjznephm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gjdiztonp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gyaaznxtl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/giuqrdlfq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gjsvpyfho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ggvprtdsj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gsbzlmzau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/ghyigpqdn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtivbmvnc.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gijrdqnwe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gihyzxjdy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghpqoendx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gexcvivsm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gegjfkbqm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gurrcfqvg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gvjytvoxi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gwzdsxbrn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glpbliwup.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gdqgxyghi.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gtitzxata.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gpeyuesvk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gctvdahxt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gadglifgi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gmaavyljz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gssqnlddl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gpcplzysu.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gizpiqgqn.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gfpquakqf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/glwcsqpyu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkahodzh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gebcharoc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gqddvemgi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ggvcyjsgx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gjbghqvmr.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gvnkcmaek.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gaodmrsmu.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gqzizbdwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gjucvbzxr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/ggqzvrmgi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghfstecnb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gezkkakcs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glpecrich.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxomepusa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gwvueqbna.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gqiunvlva.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gtaxpevxr.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gvmgjnszu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gospqskho.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gxmzuobrh.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gcgfvkcnw.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/grpvqqgou.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gokhzywsd.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gpiyhtlqp.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gfampilgo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gnybxrmaq.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gzjvjlfyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gvactfgda.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gsstpqwvl.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gacqqsiga.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/glrxvyngs.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gswvneudz.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gsmmstanq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/glirkshwh.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gwzdriluz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gxpqdsmcd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gkxpsauec.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/giqjzggrm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtrmzwtod.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/guuhspbzq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gpzwcbnbt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwklmgjol.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnqeyoijl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/guztlokda.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gqsiskelv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnjjxpsjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/geslpjlss.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gbdokaeia.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwbowbory.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gbbtqsyvf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghdfhjvhv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gbmjewnou.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gamaegbwm.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gdxvhhoyd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqgepcjsa.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/ghpdabvxt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gmmafxpsq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnstbywdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/ganmuuzzo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggspsigzd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbhqhgzaa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gctuwwaqh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsqcsopzl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggluwavsb.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gducofssd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gpmnxzvbt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gtynoaqmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gelgxoyvq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvzybhzur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gzwgqvkft.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gucelrnlo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/ggeihtnpw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gahgmyeci.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/grhmgpnop.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gxitavoqh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gdzoaqnxb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gquhprniy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gclhrtacz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gfowfczoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gemdzvacl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/geuhyiwyj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gpwkeypgk.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/grcehjyuf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gkfcvcczn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/ggftuenck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdusbvtvq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gdrbtwnmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/ghfknsxgy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxowsyfga.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/ghetdmcis.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/guskciltn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gxsykidmj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/grlywnanp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqwuefnau.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdmnrjmxp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxrgyjxs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gknonirpc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gxuiycrqd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gltjlhzxd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glqapawfh.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gthwwghkc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gceacggsc.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gekfnvsft.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gscwfzufk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqgktzhuy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gomrutaht.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwbcpklbd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvwpvyziu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwqqgdmro.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ggyotfawt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gaaelmcvw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfohtevqk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcuuuckdd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gjeqpfgvo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gjmmsflhi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gjyukvbui.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gcpjsgijj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gpwfgtlqy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/giqvayqvh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfknjamf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gksudwhdq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gpvnkbkli.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gghzlgrpl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/giwvpyxcm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gmodbarmo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/guoolpihu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpvxmeris.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gosuwisqc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmnnamykb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjrunoivp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/ghhlsembl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gspfqbuqd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdpysowrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gnrobrctz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzeggfyde.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gzaenmcls.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/goxqapzel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfkqwsha.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gjnaugfil.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsalwfgcr.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpdfxyybb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gafgirtas.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqxcddxfy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guvgccmth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbectshnc.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gvtbmddpg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gywsrciuc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/goxcdjfhs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjiypdojj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gusyksycf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gqezlmcxc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gywlcaehb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gashihnbv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gutjsyhcv.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gprbxrxdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/glweihpva.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gtffnwpla.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gvxvksqzc.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gibekypjj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gpajldurv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gxluyqyvj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gilfyeaod.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/glstdojax.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkykvhlft.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gzvdfybrr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmdscmsvt.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/geprdjlwz.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/grrjdggwn.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gwttcrdvm.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gxhmykgvf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/ggvuabwhy.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gspvqesfu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gcypdcxlu.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gkrrcnxib.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/grpdifxjp.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gfdtsgubx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gpelueklu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ghkdarnew.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzqqhupwk.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gzhfswtbv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/glkaodtvq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gzkygjjps.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gczbsxhrp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gfhkqguhm.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gllohhodv.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjyrqrawc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/goxscmzdb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxdcbopia.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbxrhktda.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/guxfunefl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/grjmfnjqn.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gddhqqisi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gxayxepeb.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gyfugbgxm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/ghsimbivr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gurodwktu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gexcqcxke.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsgaexkol.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gngxjuojy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvsxduxjb.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/ganyxisvy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gpyxwkgrv.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/giiwibxsc.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gzbmlxhvj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghydtfseh.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/geegkflfq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyvossxor.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdbwrmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gyqakasta.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/ggliwjgvc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gfbyticfc.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqimycmza.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gucjszppx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqeiidrbg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtquigxol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gefuqekwe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glkvnsrlk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gzydqnxek.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gkkcnfuvo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gprrlryjw.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gaiviyefb.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gejktehzk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gkmxkbhqx.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gftsbeelu.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfondgeqy.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gmfzfjrjq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gkcequzvb.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gvwbzfiol.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gdeahxgxl.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gjefkpfru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gioonukuz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtifpuacv.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gwldpdmtc.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gkqnvrrvn.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gymrubvmf.sHtML


<!-- 参考信息 -->