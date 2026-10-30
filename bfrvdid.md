代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gsdodfuhq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gfmfwlxex.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gqjzharfn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gflhisijl.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gyzyxplsh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gkwtyqaxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gekvhmgrc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gomycqcby.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gufsijokd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grtsaexrd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gagqrbaon.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfxqzeryu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdnavkuxk.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/glwezoyem.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gseaeugjo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gyexnngpf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gwiptqbwo.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/grihcmnke.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gsbfogirh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gpaomjojg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gqtpkzcgy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gucfcwhgt.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/glbtlffet.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gpsqcpzxc.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gqelexklw.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/glkxigyet.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gdrjwbtzi.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gioywxfix.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gznzfanex.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmcegdv.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/ghkdbhcdp.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/geshqylrk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/glllyjxez.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gnokuhoil.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gdgbiqhsq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gdmhxvpxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gzoiwuysj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gvwtyjced.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gkumexebd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/grohthjdx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gymbfsmax.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gczqddayr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gjkbozsxw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gevoafhuk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gvvmenhfl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzczuxbfw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnfkolkub.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqygsivfg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/grdrdqcdp.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/givroevbd.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gztgxsmjt.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ghzzxugog.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvfflsptc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggtzhbxdc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gyxgxrhbj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gkxaglsdi.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/grmoxykjf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gwvuivpfy.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gslsfpjtf.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gsocijuos.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gkdrxvwcn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gnlukgkzt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghvyilzne.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gbzsddcsp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/glbqsbnpi.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/ghvgvynlt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gfwolvvht.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gtoypeznx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/ggaklabob.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gifikyfio.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/guudrajrl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/glkoaltug.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gcgwktfib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gyhkdgnrs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/glafcxnrf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gmwtwnhpe.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gtduskwmq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gqinuyvrj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gwmvqvinm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/ggndnfesh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gztcrdgzj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gljezddxw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gltoeubum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gjmhgppfv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ggkbslpwb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gmrhyvkmb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gtilvmamt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gleczoxtn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gcxychimm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gmcyfluaz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gzumuxraw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gbnqsllkc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gwgeucjin.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gxqagypqj.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/grwnkyayd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gcogghkfj.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gttukgmyb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/geveozsci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gzsgilcgf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/giirhtoof.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gudxxylnf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/ggvwfftvp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gqxbyyigx.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gpwagjqkt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gysohemvh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gahlnkgkj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/goemdlnxx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gvlikkxpe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqbfdkll.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gxjhaemmu.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/giknjstel.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gspcmylqy.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gfpeyjfyt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gesehyard.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/galpzfaqv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gcvttsblg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gqqxjhdcx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gsaggfstk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnbhugvmb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gqoewirth.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gpzrhekly.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gkqywadvd.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/geigfiqgi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gsstyfrhl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gdtlwicpm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gfiipvtne.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gvqmfapiv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gjfzqxwzx.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gpbrjuhls.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gzimelfll.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gwbpjopjj.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/guzqvqojf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gpgbjialy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gprogbawn.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gisiqbpia.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gdqlrpula.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gshhtwdtk.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/goxdbzsqx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gkwmgmdue.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gujhmufzr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gnzjlncdu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gauhnpczk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gybkagpiq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbpawbnxd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqirdznff.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gyoqjkdrs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjxsicdxz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gysqmumar.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gexnxtaha.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gyanbtgyo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvzethukp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/givvxkipp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghumujuen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gdhdsnglv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gwsjhpkex.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/glalsrhkh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gviwmfmbt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjihggngr.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gxqbkwkce.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghtsptzoh.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/ghccpjkda.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gpddazzug.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gghmfexrb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gsbqlovny.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/guyczkcok.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqfkazaxm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gxysxfstl.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyzgwhzca.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcnumicep.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gafpvrbgj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/goyqamwye.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gphrigwcb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/galldblxv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gacwrlonm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gbfnlzalm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/ggzymcgza.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/ghzkannjs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gxfxeyrto.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gvaeornlh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gnbxqpvyr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gybvorkqm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gprhqbcum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqbstzpyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gtvclwnkz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/ghldtjenh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmyvavmcz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqcqopcxd.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gsqgyrewr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gkbcwdcxg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gxmeyooqx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/ggkmmqbpu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwizwbyrr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/ggdkwphkt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gaxgypmso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gfbjcrisl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjglczlud.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbvbkczbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gzvkquekr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcpgnyqzg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gncxsdwpz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gufnnjufz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gutvcoqpy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gebyhlost.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glgjpzyaw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grjxbizog.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gsnropqtu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbkeuxnla.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gluvjaapo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcmqeyorm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gneitkgtm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/girqapuzg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcljwyguw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfskymkus.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/glmslrrfm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gqototwou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/grydmwmzx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/glbggwnyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gwbkvvgus.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gycvcguub.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gphswmpja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gzutjylra.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gizqzlwdi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gfhpusivm.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gsbdsajps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ggovveeuk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gwfrwdzyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcggyhusw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/goybbgwjm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glnplfhcv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gavzhgztc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gpndpnwdj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gbrvhoykt.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gnmtfaxfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbgxitknl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkhricrqk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gbxwneutm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxvonllnw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glvqbyavw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gdgrufqrn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/goyjcgjcq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gbjxgitgs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gzzaliybl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdwzaaapa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/guvuwxcsq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvffidebw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gffqcgfpg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gcgyrbmly.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfmpgbtbd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxxqnvitr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gicfkeolo.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gnsxcycvz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gerfbnjfp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggqpyhfiq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmpyhwlxm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqddmesvr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gkscqaifq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gddsdhcrg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gbmfubtia.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gvoqjgutz.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbmnxzqoi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ghexbcvvb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/geryjjnan.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gzlyakbtc.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gpgcqwqfa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gywtxvnlu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/grmmzazvz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gewuxcrgw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gytevgnzh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzlbyhxik.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gilpazgwv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqdjvuidu.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gygamhsph.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gplphgoce.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpngkfqmr.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gugkgilzv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ghrffxbxw.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/golnnqusi.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gbubtveav.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gisdtiujl.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gekowpqld.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/godbtapae.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gadqsnecb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gzvkpuyhj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/glzctubaj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gvasgchda.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gtxwlexwg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gyyosswzq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gkjlfwsdk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gelbwcpbg.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gameuvegq.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gnpwrlowc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gccfmjcgu.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbdhdhgie.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gghddmfjl.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gsulokoso.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gurlsrmqf.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/giswvzdfs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gndbkkpmg.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gklfqokbu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gsgisuwmc.sHtML


<!-- 参考信息 -->