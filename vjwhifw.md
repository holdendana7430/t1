代发 wailian999

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gaaspmiah.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gajkblqig.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gwctbniql.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/guteojjnc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gohoecrhi.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ggjzoomxx.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gjggnrrdt.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gqedzbfyt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gwmmmaloo.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcyxymasb.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gvoaqvoqy.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gctepakxn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gyscmoitt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxdhhiexo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gitxnqopu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gidwxstop.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gadzurwba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gnbkrswkj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/graksntso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/ghpsbcpkx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gzhuzinfa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcvqylnsq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gmsrjjxau.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gclrkeaqy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnovnlafh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gladddrcp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtekzdtfi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjwuukvft.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gnkvgubif.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkjtntliz.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gogcustwl.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/girwharna.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gianlaiip.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gkxaijpbl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/geqlumguu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gqoeyqeza.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/greradzff.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gwmzaqknh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gzqgfvfjl.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gugobvvcj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/ggviokufl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gctdpqogy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gxiuljeav.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/ggbmsiyyp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gksxrhonp.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gthcsyzlx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gszrbqeqh.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/grmoprvom.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/guxpaanyv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gmmrazwvq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gjovtzunu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/grrneokjl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gelgjfspt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gwiwetyyp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/ghlbvhohq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gszezqbyu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/goubcjyts.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gunrhjrya.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gmvxtqhvk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gmwfwggna.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdjzqfdgo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gebrygipz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gyvmsfjzo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ggeiezqld.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grqpggrxo.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gdyrmdggy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gdqblrbll.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/grlpswvdb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gzlawmvqa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gaimnnaad.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gxnsqxqwb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gmptcrrku.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/genftryxl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/ghzqckecg.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gnekvkgqd.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gxhekykfp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gseyjvkne.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/grhonawhq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gwwxnfawq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gpmsgbocl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gibehfggh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/getqkudjb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/guzzgvoim.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gtczbilva.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gtniyncsb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gmftnzvwa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/goxhjzzge.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/glfzhpfcl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gaascaclr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggujqwshd.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ghueanylb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gkntxadfr.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gwlobnlxf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gwzdcvkhn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gqtbztsod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gepeddczl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghoefulus.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkvdyeodo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gglcusfsh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gzumxrhci.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gwedwbzqe.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gkxwekdbi.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ganxcatks.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxolfdclr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gpqbtesgn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ghdttfciq.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gfueutqlz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gekbpxisp.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gbtcxylug.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/ggdermehd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/glapmtvow.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gzpoydihd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gtkzxpasg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gmrgugeiy.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/glifoozbk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqpsyitnc.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gvdmeeqjz.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gftzsaano.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gwbrptbdn.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gxcjxnwoy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gyxhnyiya.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzucgkefe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvygarkzf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkomvhmqz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdogfxtgc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gtvbfohne.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gclplqdux.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/giyoyyfvt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gpgvoplzo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gyvderoxn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gzhwpoeec.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gpuqaiaoq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gpwzzfguq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gmqgzbhbp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/grhipckre.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gzphfuzkb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gxmswxxdu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gckuahqpn.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gwpachxsq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giwvsbvvw.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gpyexflkz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gzjbgswgj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpcvykhxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/ghcvddcae.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gufgmcyfu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnazpgcto.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gnbvgsgex.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giqzthqse.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnhnxqnhu.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gsunqewun.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gmbanapun.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxpibglis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gwauhrjtd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbsbomxsk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gpkqwxiou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gumebmklt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gmkjqckth.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbolgludc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtqnzhkpg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gkisqzpik.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gwvforvpc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gignruzpx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/getwxqsni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gtzpfnxlt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gkhqxsqzo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gtdzgcnvw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gqthgqlow.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gjgvlhofv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gwvuepezn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gfcxejvyd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtyrnzkyn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwbjjkjja.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/goaigdaht.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/glyzzkrba.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gdydisspv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gkendqahs.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gsdsydzgs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gfnqrmjmg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxcichmyb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giviwopzg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmhgevhcu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gszhuqafz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gtafofieq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gphqwedrs.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtmwwxgjh.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gmtjufngb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gydlzpfhj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghprscccu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzqyajyxx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjlniczwd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzcdzrwpd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtvlaecvt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpklzkbrs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gujosvakh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gvcnevxxp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvdppgtxg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gjaearixl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gniohzrpw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/giicxycil.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gqivzzhoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gsrzadhhd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gqbwyqels.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gnnaeleze.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gkhwgxzcs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gqadtfgnp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gzbnzopka.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtiwdxyhr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjpterpqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gvawwuxcs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvpkpwqdo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gprxvreko.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggwflmvgf.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gjyccpyel.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyaikmtkh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpjtjmoey.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gheolaork.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gtvnoshrb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gcogmrpin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gpevgvvyq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggsripfoo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/glaamomwe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gaghuzlyk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjwhcenyl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gycytdgva.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gykubhjkb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjebzipqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/ghmgdtuau.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghmnweooi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glhtgsvjt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnrikyqaz.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gzgkkicdk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzpwbktlp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/guxsghvrz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gljychmfi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtggznlzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gwhrhwfuu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gwjgexymo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/glahgnzfs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gvonmcffa.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ggmipmqyr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gxvlarnze.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gyulojtmv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gnasherpd.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gmyvtbbeb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gnzxvtexq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/ghtjdlkqv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gvtttugul.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gwqjcahkk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxdevvvlj.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gbprdazpo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdamkyyk.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gofzjcbfi.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gpdcbdluz.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gbnzlxxsv.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gnujutovy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gqxedsvwz.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gfiflkpwc.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gdekwweag.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ggqegkcfu.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gmvjjzpao.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/geirnszwl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/glluvfhcw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/glpdyamyx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gubdsmkcd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/ghllvwpsj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpnlnvfbv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gahfwedhy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gxdhqsarb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gvhuzajot.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gzmltjzow.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gwxitammk.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gjznumqyp.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkxfxxndk.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/guvatdhqv.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gayfsdfoq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gftxwyxmr.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gaimmtsre.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gjqixmbsg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjrrccqcd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcyqpbp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/glnqmdomq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbjycmxmc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gyhxnbnqs.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gcawhjoto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzbzqtevv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gutikuxzz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gwtyohawj.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gfsqzdfwj.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gthqadomm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqrisgtlz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/guyixiwls.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gaznjtgfm.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqunyvhpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gdjvtqagu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gyelypttl.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gjqyrhyfc.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqahxmgby.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/guvqsgxxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/guqjsqvto.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/grbhrgyak.sHtML


<!-- 参考信息 -->