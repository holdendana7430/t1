代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gsghlgsge.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtfqdlcds.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/grfjkaocq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxljvinii.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gggrqfgiz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gghzwlcvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gcqwuxgiw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gyfsxglkw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gumcnfrzm.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gibocpqap.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gqpkgbzmo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gclgtwgmq.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gwmjfarle.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gfznstxsk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gkihwfpqb.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gpolncril.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gllveueqb.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gjhmsydbm.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gjdwuxigt.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gkmjbwnoj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gzlmeaxrn.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvsenbhgq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/ggesoxaji.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gldidgrbi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gureiupvw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gqutzrjwp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gahadzjec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcesuuspo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gzubemfmp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gtuncaikr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/guhejvzgy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gshamebov.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/glnbmamig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gekzoezhp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gstixbjjm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gehfghbhi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gnweldbht.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gktedqycz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxutausvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gcvfumdtv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gdlmuegsv.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gxawwsvdm.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcuvdammg.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gkpmqybii.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvhzsffyv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvhzpkcrn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqyyufqrw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghofcqrqb.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gevxlfjiw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/glauebdno.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/guvpibone.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gfncgrnpu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/guzskjbpb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gozpauepv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gntoywusi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/grweogpdj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/grueklmop.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjwzaxnad.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gsagkcjfm.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gefbdggzx.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gymstuyez.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gluuybxhk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/grhqzhovi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gswlafvfg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gmjdvorvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gsbplrkvr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gdcpbvmgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gpzelpfto.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gaafujcjt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gziyvgtbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gunvhvyge.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gpuvgtvzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gmdljnhjj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmvkzwqaf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gildctdkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/golcyykvp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/glnombyrp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gddzhcvjx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gbzgknszg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gzrykynyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gajsgkivz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gmzhhdgab.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gczdtrhjv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gotuijybr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/golxnrida.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gipidvrzu.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gsebzzgbj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gjowldbnd.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gqdlboqay.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gknnwvnqb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnaswhut.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gyrrifbzo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/grnnqfnnc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gmamryfji.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gtvzrdkuh.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/galyvbgsu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/grsuywfij.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gbnnvplwh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gpkuuesni.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gwqirldkn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gbpkwcotw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/guanixady.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gnondgkcq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdpzcxiob.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gcxjrtqjo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gahmikcnm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gzbtwlilc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvxosuhpi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvrjmbjbe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvpzlnztu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gylcfozda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gmmkvekcu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/ggeneoewu.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/guaotxnuv.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/guybgynar.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gnmcbtwhy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/grdbwwtqi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gusozferj.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/geessnref.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gwcbbvurm.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gjkamubnq.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gmsrugwex.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/geyskaecw.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/ghcstrwcn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gponoqjey.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gwdusfieb.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gzqpttknh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gywdziulm.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gvcdtuqvl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/guzrrdjsq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/ghaqbbzra.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/ggvbjdgla.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gicicmflv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxvfhinun.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpanubnvm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkmopjjwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtxfbgsfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gkbtvbwwd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqvxrplfo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvggzbvnc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gcvytmngv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gedcqvtvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gnjsefvcs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gebxpwcor.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gskismmfl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gupogmfke.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gojqljdfz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gikscevsd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gecficewc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkrdzepaf.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gcllpmhou.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goagjlbpo.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gvvdxvols.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/ghipxeeke.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtiwgsrzd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/ghauzkxoj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gkndjyxcp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gkgngyydf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gcxdsphaj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqskwqtpi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmbgzbe.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gsasfalde.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gcrxwzgeq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gkpexfqkn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ghymevinl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gzboppopb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvpubjpwc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gpsububmw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gekivyuli.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gcixrryph.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gtxezqfap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gpklfikel.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gruilqboi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gckmckpql.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gupgddbmw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gcgzssapp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gsukfavil.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gprlosfpv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gyquetnry.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gfqjloycf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggktfozkz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/geyjwemhs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfauzfljg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpmvojuio.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gskyjwrrz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/grxkbyqad.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gksvqoqaw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gcfswxkpw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gemoghmrh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/grkkokwbz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwpxvmsuo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvhclavhf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtmhvtfgr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gursszrnh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gzlrrumyi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqrjwxtci.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gluutidmk.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gdbplmwpx.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gersgbunm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvceqfszw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpmstilkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwplwukoc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwbzfppud.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gedwhfeyb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gixlkaxxd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbeqxddkz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnncnyezk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/guwukmrcz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gowbxelda.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gpjvqrnjo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ggbgmcbtu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gxuhegjme.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gyddvkwoz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gilwkbcrt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxxohlk.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ggrkxrldo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gmzxtwbfs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gmlmubbps.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gtxvhkhtb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gojywbvcm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmwoscyfq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gnxakprsf.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gudtysofr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/ggznqnjfw.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gapwuucdg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvzabtzws.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnckwjcoa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqwrhmqyo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gpcydxrkf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ggpozrapy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gybgbjfpx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gscnmgzfg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/garkugush.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gdapowbre.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtgwxvxjp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbffwkalh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghuxfidfd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gndzrvtkr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gcphvxwyv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjdvfwhsf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkwimmvst.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvckrooum.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/ghscgdiqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gznpcwnqg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gxmkoojaf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmssdyutf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gstkiutqm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghqzddqsu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gjctgflkd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpttoghox.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gvjfkpuwn.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gsqossppl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqkfnplla.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrirlfa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfibsarsi.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/guotrxufb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gymamqacw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gfnmjthtq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gdidorntu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gsrjawzgd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfmzcyx.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/glrsfseiu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmurpmfmf.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gfnufquof.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghcvpumhk.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gpzzqfrev.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gatwzytug.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gjnkeofvf.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gnfekpkmb.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gvwvtujcb.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/ggspbhmac.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghorzwghc.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gwkjmpzcq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gnbnhyhkz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/ggxbdmojw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxhjggvyp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gtyzrzyti.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcooqpfdl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gbpthkygr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwqdwkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gqwomjxpu.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gfuhwymkh.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkdshosaz.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gjusxncgx.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwotcvnac.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcvgcdjfy.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxcjvbwwe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gnqshndxo.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gwboysymo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gkqvklboy.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gsliiionk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdgxignce.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gagxpuida.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gylltgchv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbvpptsrh.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gwnvuftak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsbrzdlrn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gocjhjmbu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gvutgzgjk.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gzcxtmevi.sHtML


<!-- 参考信息 -->