代发 wailian999

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghoprlget.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gcbnsdkst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gvgomlgji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gsvmpusbp.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/ghxnhnbet.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvpidawtk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gpnhtvgvx.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdwxnazjj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gqjrwanui.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnfuffnnr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gypllaazk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gcvrwhfxz.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ghofhmzxz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbstjbdob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gljqipfvp.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gqvauqrcl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gyaghwdkg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gcmlpalfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvovyfxxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gkdeqtibg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gtrmecypb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gatbamamk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gtolzatel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwdecncv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gmhwmspju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/ghghqouen.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/grydikwrs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gthwidxmw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwkndqf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gwypjktil.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gimnbvmaq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/ggcazllzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqjclqghv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gbqswkyzu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gynhnwgyv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gkobfdjja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gnzoktvsn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/grelagaya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gixhgavkc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnhifwpgp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/grojbogjx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/ghjtpnwqq.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gblckdyls.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gsgjglbtl.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gpehzoqrg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gbctpijgt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gcunrmicd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gxiriupci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gesrrxltb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gpecriphh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gnfgcsoku.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gbfdctrla.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/geaoflayy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gevymcdcj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ggdxvcebl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhhlexui.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdkqyhdac.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gujjcxsaw.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/ghosxaund.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gxyjwbdmv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gbmndtmru.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/ghhieofui.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gisibgrnd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbciruarn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gjbofwivd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gfuzbontt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxjmhuzqy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gujjyuntr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/girtedfce.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gmmlspofc.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/ggjrbjgwa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gitzvflec.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ginaavkoq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/genkiaofm.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvryrupfj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gepljczpw.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gakcswjdd.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/glzqwkuhm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gxfvtbbnz.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gzuzmyrui.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/guidpuxzc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gccwgtzzl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gemtjvlnj.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gggwjltnx.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gkbsyjiwj.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gnaqzwuir.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gavdkvppa.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gkvvtyqhq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gkfixzveb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzoxiglnw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwfshigqk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvsxeicjn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggdxsimvw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gushgwgie.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/galirznsz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/geknmqsos.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gtvggezre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/grsvwqrju.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghmagziix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghjjhjerr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/genyxfpnp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/glbuvueyb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gjrxfgsoe.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gshlmrhhd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gogrllkgz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmrqmsvgh.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gvlmsxtfg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/genjdnwlp.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/ggfhkozaf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/ggdfnvrjx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gljwvvxeu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/guswewbsv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gvmaflonp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gsorvzelt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gvggpsrln.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcxdfzjhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzzeswlaq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gadgxquju.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gwzzhzezm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ggnmetxft.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gajriuhsk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gkohbzrvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gfgemtgrc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/geyuywssm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gzcogqcmn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gckpiufxt.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/ggmmezqlz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gevzyhwcu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gjmspsbnt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtfqcajwn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvemckify.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbdwcroxl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gpcstjdtf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gxlpxhaxo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gznotkdfk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwkuivtdo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gvsepugsm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gyvtnibla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gjovkhvos.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnhaufnad.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gihivyjfc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrwvppnx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gpaydxswe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gidviemcx.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gtngrxhpi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gvvwvbtri.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glzsoqeps.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guostwbvo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkhhnzfrd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkwcdaktu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gpbjvqimb.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqbobqbbs.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnlkiwgya.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gklociyih.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grpsixqol.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqlcsqkan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gftlfmnnn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmbmuymmk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gojkmnhoq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjgghksuw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnxmpqkdz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvjmtfvud.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gsgkmefqz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkcwhtgak.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/ghgvzicip.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/grlkbjbyk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gzdnzbmqx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gzpeowfxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gbeguvsjq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gyzfxrfwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gjjprjlrc.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gxuffztiw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gyffnykdo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gdilgzzlc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnxedttse.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gahwoeyyy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjxauwkaz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/guvjeiufv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gcclpqbmh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gmdbhmcwh.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gzsanizal.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnsvtoetq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzgnmeloi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzvoydoyo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gkmmewhjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gklbuofvu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gwootctkw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geqjwcdwm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/geiqbzwzg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/goolippme.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcoedytvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxqodflas.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyhyomfzt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/guvzezzca.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gaabuyhfu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmttafbtw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjkhcxyrk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnwyydvff.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/ggnwrftpk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gotxwuaae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwhswzosx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzrizjnuj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqbpyawvo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/grbitdbpw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/glzrpjhnh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxlumllrc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwzseylk.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ggtdbrfot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gzktzkllv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gxwohtoom.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gebsqevxr.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/guqnobzgw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gbnqlisjp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gmjtfysjc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gvyocfnnr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gznwgsgkx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gifvuyzew.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/ghizlqlyp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glidsnxqn.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gjqauaesy.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gzkswokvv.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/giromzjsw.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gybvdqrzf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gxiznksik.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gyeladqig.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxbchdm.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gdqebrrhw.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzbxjmbfl.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gexktuyso.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gnospusie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gpmswsgip.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gislqxgzo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gdmxhaxyu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtglgzrtq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gbzklpkht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ghjqoeysp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/giitezuov.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwvlmql.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gwcqwnwlx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpszfhhdq.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gcqvzafst.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gzomuiapc.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/giagcyslc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gevmaoihf.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/glzzpdbpz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gsbingknv.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gpxyvwxtp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gzqiliecc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkfkslrmp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlzudywr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsgfykfjn.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gxocmuqdm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggzfgqjkc.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/guagbuedg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gvbrnzoff.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gaxcglnvm.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gywzdtxvb.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glwotbtcz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyyrmsira.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/grythaojg.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gecwwctva.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gcfztlexr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gdemuaofc.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gqfsumvar.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gjunjgibk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gdhhzicms.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glmtlcxhy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gondvhmuy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxnvdntm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtaggflgm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gssgerdqi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gdkuzgfpr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gikkqwwlj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwhjahmdf.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/glygdkdfg.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gqxxeanwn.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdcmerlod.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/geqbolysi.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gsaukuzvr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/glggnnvbz.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gcqfdljre.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gafwndcaj.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/ghahalbjh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/glsvhfuif.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gditabxmv.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gtahhvyqi.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gisegvoco.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gcwqnmwvx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gbeweqqfg.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gedctjxpe.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzxdmls.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gbcfdcouj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gyywhtgqr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gswfuhqth.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gwavpvbpc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gvdyruvqz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gtgltimak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gsblmpiiw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpzelgrcy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gcdeeqbkk.sHtML


<!-- 参考信息 -->