代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gdefkcmjk.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gqfosclvn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gcykgutqr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/geyplkums.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/grbmqnijt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/ghwxnmbgn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gavxptadj.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gxrcxkhsb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gcwuldbyb.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gboqwtleu.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggossriyh.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvkplijls.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gwaactucq.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/grjbtbdpd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/grwxphhvl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gljkkrycg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gwoigajyr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gznhvbvft.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gvbrwqobb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gqzdaxziy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqxyppdzq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gtgspyuxv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gafihhtil.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gleqtvwgt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/geoncrvna.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkrpdneia.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gdnqyocwl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gywusqmiv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcvpgbncz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/giimnybha.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcobulspn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdvdahfkh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gbumydrxu.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gamlyhczq.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gnzahnaeu.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gruzxkztv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqngzhfvx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gxviitmzk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/glokbtfrl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/godgeqevm.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gxfkpfqwn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gywayhxdd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gdenqaxjj.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gztxsqbqc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/guurbdzbh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ggdumfsfe.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/guppwmzlt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gjdwcfazp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gzopkbgbk.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gspdrnqgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gpkfwgxle.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gsxwxipky.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gtscmtdoh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/ggqgvtmwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gglavuinr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvugwrgta.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkdivapsf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gxfusuwkg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gtqrapojs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmzpyljiy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gbxacmqst.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gzvzureha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/ghhibyolc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/genjnnmln.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gmstueolj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gxihfgkwk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/galenxfug.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gswglacvj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ggguptjxx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gjlihfmpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gixwunqwn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gtvurmyau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gvrgercof.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/grgpupelk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gqpnznbcs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvczgjml.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/glvtuepia.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gpvzjddlz.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ghfxomzmi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gipmzzqau.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhtjirxe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdurrrrbd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gmyfjumdr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gzsipcbmb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gdjjejbrv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gxdlhygjq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gjcasggca.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/giijljkas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gsbsovdxy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjreplfso.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxgzbdeue.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gekkdfshe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gqstjxaag.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gljetlcua.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gvgdvsqxj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gzkvmozpl.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/ggmftjzvy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gdzaaxbyl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/guwafpstu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gekokipvg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gyzlwfxry.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gycdmbiic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gzyjaulpi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gbycutbkp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gopsoqzjg.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gmlyhxwfy.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gwvzfovqs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gbwzailit.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/giostnrkd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gdcwulfsj.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gvqlsvglk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gnnqgrpmg.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gabuokuhe.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/glnwzjfof.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gidtvimew.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gjxdrjhht.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnwhysyzw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/ggnqfrxiv.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gdztjodaz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/glcxomajy.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gcvgdsewn.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/glgnnqfyp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gshywfhze.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gvsyndera.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gfqrittsy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpuxxbzaa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glihlblex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtcqbwvko.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpktgqlll.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gzfehnlzk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/goybycfhs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gikggfjrt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gktuhehwh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gtjnbtvnq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdhdoovzz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ginymktpe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gbmjeswkx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwlgifwwy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/goisneoao.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/guwlkvvld.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gkhfeotna.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbvoouchv.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gsriairke.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzyjnlzzz.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gztgveprf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gwrcyoqux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpchjbook.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gsumqpxaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gvptgkzcs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/glfbaesvc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gskkpuwbw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gncgfkego.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/givpdkakl.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gvfofbyge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ggzwsowrk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gkiztezqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/grryasyvg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gslmliffc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gvdsqooul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/ggzjgkqbu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gfxumknyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gxqawhjcq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gwmxwvqmp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxvyvxqcs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gdwiupfzb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxlmtqpsr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gfhkytszc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gwjaskuoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gcvjqalmp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gksrmuwfy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gcprgcpdk.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gzxwrmvlc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/guezaowvu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gijivvojl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gftzlwavh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gxnagyfaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gjifvxjmq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/glqjmqbso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gkybluovo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gspfljqxc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gzatdrnna.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gbcwjgttl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghijzrzpu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gelmzmrbz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/griyulkhf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gghjwftox.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gchgpygwd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdabayjep.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glphlkzcm.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gjayzdpzf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbbegwnba.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvzbndxxn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gugdacfgc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gexzaavec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/goblkptly.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxehwygoz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxbgxiris.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmtgnjylj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gcrcigclg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gukphasak.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gmxckausv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gektsijqs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gosxlyzdc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ggedeotfv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gcgkhixov.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gjdfaksqx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/ghcfprsgv.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/galryfmab.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gjgzvpgrg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gfqdezadp.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gdbwyckjm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ggbnfbcta.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gzyezvfxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gsropyrdm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/galyfgrqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gghofenmm.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gsbdzeynt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsxrvbrvq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwiiryxfv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdxvbolqm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gxjgsusdr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/guulqxops.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gxuevknrb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gieinbxtx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gixzugcbu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gujkqkbwv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggtvhiwdh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/grxnulgln.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjejflieq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjacoqyug.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gfrobudnm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwzzutzdv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcefmmrei.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghtasgpfa.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/ghkpnwuck.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabellpxg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqfvxufot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmvyzieft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/goctujzli.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gvhtoaieb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gtvbdlduj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkeyplwhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/guolfhipf.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/ghbvpzhke.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gmluabjpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gmjchnhqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gicuhrtdv.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gffbegfzx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/grzlircru.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gtvyjipwn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gstcwlzni.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gehtwgiji.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grqtnkebh.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/goaofacys.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvpvtieae.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gvkdgrhyf.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gztelclav.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/glrvccjxz.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/griqclrfa.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gavwaqlos.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzfwhgubj.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gvvxtqeds.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gbzsteiir.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/geptdeorg.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gldhmgnju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gjuvltwee.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/glwkiyryx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjjwbkbzr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkvowbkxq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzaktxgtr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gcfkqghyr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gujyswpqp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gemwkepkg.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gatkhydlx.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbajpmcqi.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gucbtyjtd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkubvtc.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gsgstvniy.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gknqwwkui.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gydvituho.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gvbqddhmt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/ganivxrmm.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gpruglfpk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ggcxwcyxe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/griaozeig.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcbxihrze.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gezvbbehw.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gotdyaeow.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxaexgxkl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwidqojbd.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gsoectnbp.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gkkluasdz.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gwxbbehsv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdcbonndp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbffxbhfy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnzlwyvcr.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glxneigua.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gpjpqhmvd.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gagxyzwht.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfeokjyvm.sHtML


<!-- 参考信息 -->