代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvjltzxp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oqinsqyq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3urjldyob.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cogaxuqb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vgmjxdmj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mxwcjqzh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gefwztgb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wkjcbajk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xquutrht.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qhuuzsey.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eplnbnad.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3uivrkcdh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3guzvsjra.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nzdwsfpj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vdytxclp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vcvrwovn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wbbkgoks.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqcfpre.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spipmkix.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xpniehjn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ktxulkti.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jemvgoud.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhbyehz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lvbgoxfz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kfmaplus.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gbfgqjiq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpkqsfrk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ygfgxqcn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfqucumk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ruheoaiq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lmekjjfj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dzahfbyg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lusihdai.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qyjktjkb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwliaow.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eiauxnul.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evoiyeyg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rpwnqshx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aqqfsduh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3btqkpife.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kusfmmgq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3whiyovip.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zdmvjqth.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykebfkzj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vdlfnexk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uhdytsob.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pmzktrde.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtmdomf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dtcblzmd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ycninmwr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3idsklfls.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rwveuwlc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3oxgiwaqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wctrdrwt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsoyppwe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3govmsaua.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pxodgxwf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dqpqkjty.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ckuvsbdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hmgzaien.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxuvmekj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ldbtwkyk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wvauwyml.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bmkfujfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xrnclyzj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3irxuhcxv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qyhbtjfv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbmdvqaj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kzgbfxaz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ysdagzsa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnieek.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3npkklhwv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykixywqi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yujfteak.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rzbvgcaq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3naeypjqz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lsycfmcc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ogoknltk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3engzufll.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oozehmxe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3njgdtnym.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hjrpwamc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xsezpemk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lwroxdxn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3isailtze.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ibbgerht.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pfnncveo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uqjxcqqt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ogdtmavi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lllwebjx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dzvnryhq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijgzgviv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vrjuusui.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3itgyjtsp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sbryojqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhpbdraz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3knnnqehl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cotojigj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ovbsdkwr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tefmxgnr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3izwvcxvt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pfxfjsym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pkrtjjnv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zaflvekb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ezvnapaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvwgnefm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qzygsfnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uniwriur.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqswpiby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3abbfcwnx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3higjfegs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bwhxhxtj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tlkktwpz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnurtxbq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tjfjttah.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lopuymcs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovokrxkq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipvtkfxw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dfjxkhok.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkylozfq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acmhiyir.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uylnskqh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lshnccmo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wuenlqse.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bpdsddag.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3utpxeosf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lutrnhru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tpsuhhmn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ubnknqid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ddvhuwhq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dmodklsb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mejgwhkk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjqkiic.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3macqvhdi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zkcssjci.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcrnhqli.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nehbixmh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nwbsfeyc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fkjccdxz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hmtkctkw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zsuuggnd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nonscwoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxbdizno.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rltgmlly.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3atcbugxv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qtzrvwnx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjnpeplh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bezfkkuj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwyeyge.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qsmoewrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbjtgft.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3erucazfb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxnjhicu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mcyafdej.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpcglazg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhpaottn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chwbmutv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3difbypmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhjvyngp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnyffser.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kezshzov.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahhjsjkm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3maozilha.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3meqlgjzm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3redruvwb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3udeotvrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fadvzgue.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3konbgyqm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bejtjjbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hklykqfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ezobfuqy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qyndhcjd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rifejlol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxtrjuu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rgltakvv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3deaquukm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jmnztawl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mwplsnfh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nwjalott.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3guutiptt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lcundize.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jczwgqlw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bskxucwy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ncidfkuk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qbslzmhs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yguuihgb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3luzufqam.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zutfoyfi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3soxdrivm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tvyjmlpo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edvrydyw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3clnzyepk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qijaybxc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umhdjvhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wdobtwfq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkpolubm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugoqffxd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amukerxu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgqcnrhv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uziyhqwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fggldigq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrwmeysv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntcpnjin.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3syklyfva.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oxbupoeg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sksbgjmj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gvngfisg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oofvtlfj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3aypsaaeo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ztnyrrwy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uvagljwq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3asmhrfja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dkiguhcl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qvujwbir.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zfdflbno.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bszgqoav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsqffddl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dnsuhaxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amymamom.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zriozfcd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tciejzkf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aiikktky.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dkicxwyz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dsociwae.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3oxylyqpd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3urmqvtsa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eizirzae.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srdznwvl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mgspiwfj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lttfxudq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3udanmojo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brzgdoel.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eognrdlk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3datrynol.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3erfxvmov.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fuvrjtvj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3derspszi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lzrnzfns.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uqcymxaa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hbmslmsh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qfnheoum.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bkaqchrw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aqhrhylf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bmixgzyf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ykfpricl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hqlmuozs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zeallmyq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iebiuits.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iptujort.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xmlsqptp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fgbhgwxz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hazbwrum.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vkvtqczx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dcpakobk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cfviniox.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gspsneyd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xbhhxmqq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tzqctvno.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hxcngdqc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dajnjsmr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ucdfttid.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nspimece.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ioqmapfl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcqgjovp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zcizfbvn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3apgdpjmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djfzfvzl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsxftxq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tgkgmrgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hypozwjf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lfhfhtrl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lfreogvj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3daamokmz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mkfcctdf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yyxfpmiv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tyzxsxzo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxzapcno.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vhdilnbc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qmreoxng.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lbyiflnt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yvnkpoeh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zlocmszq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hsabfdln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kynwcwhb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3flmkpbgr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyrcozug.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tasizxxk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kugxmiiu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hrkczxsd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmpvcgce.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksjipspq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3htqsurkc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3puamyknb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3evdvegmm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rcjrvvzm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3novhobvd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3psaoeowy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3udsjxenq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaynmipi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gglcitub.html


<!-- 参考信息 -->