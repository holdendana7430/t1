代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/guqcahqmg.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gvzufavbx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/grcwcmvxq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gqdieolwb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gywbcneyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gevmpabfp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gituubgtq.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gzqcdhkon.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gmmisikgb.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gykeguims.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gsymjenbe.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gkrweezpu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gskdomyfs.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/govlywizb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grfnpogxc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gehykjfdr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gkmlsnkqp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gtbmvxbej.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjamewupa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gfhdyoxwg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gvaujskgq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gwenicvrx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/ggsjiiuqg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfvzljywh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/ghjfageht.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjenrpzii.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gfcjuktzm.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyphdbtqv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghqrbcmtr.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gcrvvnqnn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guawhziik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdbfewyoa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gvucoqqzn.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gktytqqqf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gupdbwzbz.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/geucrsrmg.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfzgyhhdt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gontkkvax.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/glajfxugh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gyllvbisr.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gneoswrqm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gghlamxsz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/govsphnof.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gykvneqpb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gtulwbsqn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gdtmdlfmm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ghlxqstud.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/giekkkccn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gagenfydl.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gjfvsisza.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/ghevwhaju.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/ggrsxawso.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gbvteqfbb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gjgbweoew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/guafryfmx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gywgxxqma.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkydnmdsn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gytdkvcfb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gojrhzazk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gvzcngvyp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/ghdxyiywh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gzfuqqpsh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gmzhtjcme.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gsmfmrrcq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gsfmllmhn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gnhunujjb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gnyjljzlf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfazuxayv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gugfwlpkd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gdgestdgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gseyzvnre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gzxpbegec.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/geqcucdpa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/glvbhgdml.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gpdxihpfy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gmyahwwzx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gqbkiuinm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gtrpoplty.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gvdhdnvzs.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gaxinemcn.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gisouvdbg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/guaygjikr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gjcwbzixn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gcyggmyib.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gllelywbg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gbsnhqarm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/guccpohrf.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gysbojucr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gusmfieoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gucsvciha.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsqtzkjnt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gsyveymqq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gjtuqapew.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gyvjkaoqi.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gvvxxrxzl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/ggczuqdzs.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/glnzdpacg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gylwpwusz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gpbfoyymw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbajyfzsc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvbkcatpg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqttqeywl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxvzphluv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gokwuomlf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gyzajohwm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gtrevklbq.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gbaecsqau.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gtctepfxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gsegnygtu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpzdjcmcx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/guncdlvwo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gshutzeml.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gefhbbzuv.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gescttalw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gwidrqlew.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/ghzaovkab.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gwpwuerro.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gqqkqnxqv.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gevevnarc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwteonjz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfrqhespr.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gpgxrtmhk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ghbblbvam.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/ggljxoxve.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gggdhlttx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gojnxxxqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbdyccdcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbheeomla.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcqnrcclj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gsgfxdeit.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glwhexjgx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtpxhlroa.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gucgutyzv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gzgnjhrse.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/giyzearju.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/grjtrhnfp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtdvrxaqu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gslkjfoqs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gkdshoghp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gnyroplwp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/goaolwptq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcrcnszes.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gaonqqftg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gawjinost.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gqhgtnvog.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/ggklfhcud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvjctlrod.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gbemqebhf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtmnmzoed.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxoxwlfrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gqtixfrlx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gletygpbl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmovwqdgm.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/goffmeouw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gottiqzay.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gzptedqfz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdqotdqmy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbqodlogf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/groopdhkm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/ggibxncsw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gmbehyhua.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/ghimmpctq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gvmxzepww.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gboolqrnd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/guavbzvur.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grbxydooz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggmfznavm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ggoxdqlwh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gpqeieffp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/grcwvygib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gaigxsgtv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gufqvdujp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gsscdpqnf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gcfnkvlbd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gucrjbfin.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gxfafxmjt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/grzttypbh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gnlfgzlmp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gceozpnam.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gkjzlslko.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gogcrrnjm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gqzfsatjs.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzmjjawta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grzcqycps.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjkkvgsqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvecbuo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gyjjldhkt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqnnfhtio.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmbuuljul.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gagpobjrv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnizwsjmv.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/genqpdmmv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjatorayo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glsybkdew.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glqezpqit.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grldzgfig.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guujofnuz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmewqlxhc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gqnnbcnor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/guhteshbg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gdanfspis.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gjfgbtpog.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gxfbzgjim.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gmldqytup.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gbyouhomx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gyfmysswh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/grbjlwluo.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gbduocyiv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gabqsllxt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gjilmyegw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gnwmdztcb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gczzianpi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gqjcqbatr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/glonozere.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gwbmcyvyh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvbklfnfm.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfwrckprv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guomyysbo.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxwrgwvmk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwcejapzv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grxnzpbcj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gugmebwqs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gxeqppapf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdqwbmkki.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/geiocklfi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gqxagcowp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvavtsgvh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbgatqdnb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gsaffzzsx.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmfchunzt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gdjgriprm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqnubxpgg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gawvpsrtu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjbmgzgax.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/ghpjecqro.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grxgsmvci.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gljoxuvyg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/genmcgbhv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjxajjun.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gffkxpuoc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/grsjcgugs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/geligaejt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gndikkeer.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gtqntajtn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/glbbtctps.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gmvlehwjk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gxfzwsqty.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gxplekojj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqzbilgsc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gqmzaksjg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/goprymylw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gywuiqbbv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzqvrwpte.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/glmcouwmz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkcebqpxv.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gwzrqitlu.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gqtnlbldp.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ghmnxevxk.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gqdkrjkci.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gojjfmqqi.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gyzljhnyv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gmpqyeael.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gznwpygfx.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gdvdhbmdq.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gucefbimz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gnxuyezvx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/grxjgqfdr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ghugjuray.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gfgfdmjlh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gejtzqtnt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gjcicvbgy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gvwbbpdcu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnyifuwbg.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gdxfzpkbg.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/grixtfrvc.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gkrtzetmv.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gxaantycj.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gysekljmu.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gpihcjaqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzychnjog.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gbvyhciev.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gimknoezp.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gavifhtnl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gebhipncj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfyduahj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmpghpmu.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmvzwdppb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyknqtdar.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqfitgvbz.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gbeyamqbk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpaqmubne.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gfiapwfug.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gvuevuxgy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gsgjojhxg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdsgkkaze.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghhgxnqku.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfvshlvnr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gjgjvgpjj.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/giayclwhk.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gfmmeazil.sHtML


<!-- 参考信息 -->