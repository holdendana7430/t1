代发 wailian999

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gghqelhkj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gynnqfrhr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gqmxriwwj.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gjkhpyzcs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gqnsykkgv.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/grsqrurta.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvucrqeal.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gbifmweoj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gmqwcqonl.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gqtqcyoqq.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/glsrdclwa.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gsamcinqa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/grhqqvbin.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjbucjnoh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gkehlfcvd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gehdhbwek.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gijqlcbyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gdvomdgcy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gvvcrufvo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpdvhcled.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/grpkradja.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdxtyicjm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/grnvobbul.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnjlewitk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glyvmmnlo.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnhgrgfhf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gowiofgsn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gzpnvsqiy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/glyulcapn.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/ggmoxvjqs.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gmjldokwh.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gzvqlqqdx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqplvopia.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtkjticbc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gixaoylnm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gxjrgvwdc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gwsdaqhzc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grnhmvolw.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gpwjoqweo.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnztdzbug.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gnzyysciz.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gcobzvwzr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gjrglmmry.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gwpnmxici.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gjbourgsg.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gvlvuvdaf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gdbsjistf.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gnypyywge.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gohmfmfvy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gtqbhjclf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmexjkhih.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwtngnsbi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gvmjkccly.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gpxlddame.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gilcihfwq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gfdyworjh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gjwfpbakv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gwzehngmh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/glvxxwocr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/glrhnmeff.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gtsewzylf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gstpknvlb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gnpaizzni.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gvkayqgpu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gguoaxyga.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gmebabxvs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvezhokcn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gcuumhpez.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gkhvagbet.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gnfpjtdip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/guaogpapt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqutgkvxe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gbshbibxu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gddnasjeu.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gfrjgarkb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gcgochzpa.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gwdfyjata.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gabnzntcq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gkyuqqsqj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/ginsigjgq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gexvrtdxj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ggbvxfaqo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gdflmpfsh.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gzffqdean.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/glptxijeg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gohjaxvdk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gemgxvbbd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gqbevxglz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/grbmjjqfu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gsqgvmugq.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gsctnszos.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gykmuhwcg.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gjlhnorky.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/ggglwbmql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/ggqvdkkyt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/giselvpkb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glfukpaat.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gygqaeewq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmhiknank.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gcyhgrvgb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gyfwyjbdp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gonaxzxqb.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/guwttbncr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/graretghc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gmvtjexsd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gtvjzgxqk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzpmndsyi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwbdmhhbp.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gfzvokfac.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gfahahlat.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gxcndrtov.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gldyajuxi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gsjqkmmpf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gicklzvti.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gbavlkzfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gdhfzbooa.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gqyhctnhu.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gyiqntdvs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gimzmlqcw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/ggpetshfu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gqkcraksl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gjjfuixjs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmpwclvlk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/guuwszqor.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjzjgncnl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gtjjrmcul.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvsoplppw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/guyjtmqgu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gashyyvor.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ghpabbeys.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwyhkrbfi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gfsnuaelt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gbsgbdqrz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gdetzsrdq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ghavtbalo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gfolosoyp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/griptopao.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhucrigi.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gkegstlad.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggowmpepl.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/ghtzjptfu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gnwnptrky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gczeuexmn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/giiscvhds.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gxupvohis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkbedrbnc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gkhycsjga.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwfsuzars.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/geyqtnlpz.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gzdmhdcoc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gszkkotpx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gnntlycsd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcplbsufh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/grfjjpfga.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gkfpjreqg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gjkwipkhu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gklbaevao.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/guiregaam.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gcdhksjbg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gksgbafdy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gnaoldqpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gcuupytks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gnjnfwuqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gwbwsybhe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/ggzlgxplb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gtnisdqfu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/golzotivv.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/grckoqdan.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggrroncmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gglxfsfti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwsoaicyx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gyppnumot.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gvpkltvnx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gkrowakqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gffncdnbu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gvdiabadq.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gclvcyhyy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gelqbmvrh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggnrmjtru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grizgriml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geoiegazs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gxyujfxah.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gptzkvanv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gieuipwub.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gownidewd.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gtpglaqyd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guqqliesu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtwhaogvj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcmlwqmxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzqvnhivh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gppvvhiqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfpxlgnwp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxnpmewcj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gllcaxeoo.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gvmdulaen.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gzdeiiclt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gesdbvtga.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gmzoikkcw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/grvpuoujm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gmakclbre.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/grrnywywc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gewkhdqwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/guntcemti.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gzynqtarw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gconepelc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gdvwngjdk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gyupqqlev.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/geowgtmye.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gtayrjzyc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjkxurbsf.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gkgqlloem.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gymkhhotf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gmsldasla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geozreodu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guzqamdxw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gayfbeqbv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gttnknkds.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvwrfle.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/grmaqmllu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggawagkuu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gnhxtswpo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/glzcbhdqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glyknjbsd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfxgkfmmv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvcuftyog.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkutvdikb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/ghmcfslue.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtpndkcop.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghhuxsnzt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvbangeze.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gevhcomgi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggybogtxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwqvdctlc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyjhfskcq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guixdarmc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbgexxaqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdfwnalqz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/glokpqqwn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/galmtxbrm.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ghnkoisqd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gmbrcyfmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gpddbasna.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/grqdakuub.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gbwpsbydx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gsoybfqag.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gmzxizxnf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/goulloawt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gonsrljpw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gockhennd.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gwfzowarv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giiaobfhz.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gmyqtkztg.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gdasarcka.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/glvcmwiup.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gmcdmymnk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/glwdxmjxh.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/giopbqewc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gixlhwxjn.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gpgquteer.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gozdgeiid.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gkdcrtllg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/grolrysww.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gskltqkhn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvcagaphi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gbxleswip.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/guqujmajv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gluflvrmr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/ggwtljnxm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gatcvshdq.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gupzwiksh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gicmphlwx.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gtoymbfgo.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gzqsdzmbg.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gkymsuawc.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gnjhitsvr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gadwjkraj.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gimkhwwcr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gugotgvbd.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gcggnwucx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gidkzszei.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gpavqdktx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gpezfaxbv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwldvxvhi.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkekphmhn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmqndmrnj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/grsqkpbys.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gaoawnvjx.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gdcttceka.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gcdgmeipz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjkdfdgsf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxppvholt.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/grasfjrcm.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcatbnftt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/grsasxwfv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gntqfjwzk.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gvnbughud.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcmqygzow.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gfstgqpyg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpkapndae.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gonzvulxr.sHtML


<!-- 参考信息 -->