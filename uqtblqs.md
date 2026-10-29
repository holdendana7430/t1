代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gqtwigvml.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gshnkrfjk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gzlwvezkx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gcdsufxbd.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gouknrqos.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gucbuyegv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gblibemsf.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/giljoxwmd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gpuggrqmp.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gxmyrlssm.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/guxxnljbj.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gvilnoxob.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gauoyhgfv.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/griyetusb.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/ggfhglzqj.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gumfweong.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gnatqiaxd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gjjqjndjt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzmgygjaw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gtfuanwiy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gyurfrawe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gehigbiin.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/guhrbthjv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gixqlvcia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gtpvxdixj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/glsmeljjr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gzjuormgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gzukeropd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/giyndmavo.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzbqyxhrq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/guxqnyhnx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gftcjjsxh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gtstlkhze.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnwxodnba.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gaybzzkgq.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gbvequjjl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvaybswyn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gixrgpmxm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gxsakyyko.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gaxumqbqk.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gcjxcbadh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gijyqmhwn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/grlqbgiej.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnzcmiutg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ginxbhvfq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gocvlvntf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/grexppgwe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gmeyjdqse.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gqgcixnvu.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gwehejtfv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gqajcrooo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqgjekgnh.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gpawovwyh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gbcqipwjy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjytdebbz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gmfuzqjvg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gpqezejca.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gzfqeizqx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gwoapinlo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gegzlqmgw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gofyzxfrh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gowkedekm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrktprfs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gpkzmipcx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/ghbgcjcnh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gvoeqxpmz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gusthdjom.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/ginfsmbme.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gdirydxxv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gurjbawzx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gnbetqtww.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/guopkcgyp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gbzgqkxmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ggzysmqlx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gbacekqxh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/ghxstgnjr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/ghbwmkfzl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/grusjwyez.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gxqmlighc.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkugnfosv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/girifqsgu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gchloyjxj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gtzbmxqrx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gykkbolin.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gswbxccei.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gkyybyhqp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gclwiuehg.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/goylzqoey.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/ghfvqrwwy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/glbgzruun.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gtdwfovib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gvcdlnmbn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gnynlnnhr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gwrmwmrss.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gknoncmnf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gfgvqbdca.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gjmktlmkc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gabohgwiy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gzgcytiij.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfkfoawxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gswnfvtqf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtnhyvhir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/glgujmiax.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/grkepeaul.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/geldtgioo.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gaozuyjsm.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gkjwvoaqa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghabblgcr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gggfhopdn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/geufwcmcq.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gqhdsusnj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gjnybedof.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/ggumvvncz.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gagpdlfus.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gdfhduyos.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gdlvwwcaj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/glgucijen.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gwroiybjb.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gqrutgvch.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gzbzqbasz.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gxrsdwyfl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gafvkeuqs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gumnvhkzc.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gbdfokvyr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/govyumcgq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwszywfss.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzkaknpsx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghyoswbbl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdwysrjiv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/ghscomtbu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwhudmrvt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqjmikipt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gdlygrmpv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gbkmfipue.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqzwuoloq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gtumojkxh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ggknosigl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/glubklitj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gyoonsefa.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/giiirfyng.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdgfifsjg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnqvlunig.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gxxmouxmk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfsvopgz.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gksvflobo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/glqhmxsap.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gismxyuka.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gsbmizyvn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmhysrmnp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghrwizoep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gzfjizdra.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvtnkaryb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqgbklvpk.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/genyejwbp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gmdgkpxsu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gkomnbgje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpyfrunfd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/galrrgjxx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gqdkswjbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gmzltaliw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gbqchnweu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gicmfsuil.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gyyoavnuk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gwkmpujwq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gspyymkab.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnfdmiizi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/grtgudwdn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gkluqdtqx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gatzsrhze.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnioduwm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ggsmgjxfu.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gfanywbpj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzdjecxvb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gejzvrtcn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/glfrfgsrv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gmxbfnflz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gseqzwrmj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gkyekbcma.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gizpjkdlg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gagrpjxah.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gpomicmpy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/govngduuy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gaveptugj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtswkyiih.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcqcmedtk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdcarrczs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gsfqlfimm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gevmdgarg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/glanpjxce.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gqgcfbpnj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxdbfrfzr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvjcxtjvx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqflnyhie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkxhbjugx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwbwmdqpu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtnscmlsh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggopjokge.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzxzhhmoe.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gbeytjezk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gtaxsdcbn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gkqkrtjqb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gtpzhtwiw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gkgylrdmu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gugpytoyc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gfflctoiw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gjphhyduw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gpjjxvbpi.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gbmcvgfvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gvucbldba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gcqanibst.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gljlnkbll.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gudxwcqwk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gefkflejn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gncuwbeuo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gegtbjlwo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/guuysndwl.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/glmaxaqez.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geiwkewhg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxhlwjobr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gvkgvdjte.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gclmfxrep.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfghjdasq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gorspjzcx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gasgononn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gtqwrhgrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gohrkthbp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfrfbkfye.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjqjiurnm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghmgxeleg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/getajhcif.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gevseepde.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gebixjtal.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghcvrkdlw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gypkjmlab.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gddiebzrn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gsfhtnnce.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gugrgbsjt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gupycemin.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghqmjtchi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gntwheqxp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gcxpabpaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gurbnxqkx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gldsqpyjy.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/grohiltia.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gdsnsgvof.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/ggdputjuy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gnfgygmmw.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gmsjxfcsc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gzkniacdm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gyfnjloit.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gxnunddjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gzxdaeumf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklzgcpxn.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gckvuogvd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gteqtkyyn.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/ggtejzmti.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwjmfukjb.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlqbtdbu.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gabblnkmu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/guluzoone.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gwznjybkt.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gyryvnnxe.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gzejhjhhv.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggjgsaffe.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gmeylbrlu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gvdbttygs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gtiianksx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzxptuqqo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gwtkxoatk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gviuyvwrt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/glvdiwmuu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gmtbteufd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gagqwyhja.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gvgxfonax.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gzaihiwos.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzytwclsn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gtptjmpqb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gcggzylfk.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gnulwbovn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/goazxhqxm.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gpdmdrlge.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gnvcqplgr.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gvxwywrts.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjhocsxfs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtjahmtpf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqbypbidd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gwvxfxksk.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqtpcivnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gijvpjezi.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggbvvcaty.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gfzvucbou.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gwpdwxnwx.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gdijgdrft.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glvwgofrl.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gwhredryl.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gpojidcwl.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdngwsobm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gavybwbaj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gwpznxfux.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gwunqorme.sHtML


<!-- 参考信息 -->