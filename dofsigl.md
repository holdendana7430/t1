代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/glxjgjdjo.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gpqgffyxw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gsksmazao.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcudoxwmr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gktgtmflw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gstidbrjg.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gybvzbukl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gpvnpthxs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gymigsnyk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gtqxtdxrw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/grlimqxlh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ggiourtnn.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gwurxpkte.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gaijsjtfz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdrrubvya.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gcezeeggs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gqvtsfgns.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/ggqivitsu.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpxaiclwh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsdruqf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/guhphbfkp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/ggnycuczn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gdvmrbjqf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/giiojycuj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/grqeujxon.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gnoguansg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gyzuhtkql.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkruuxafn.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gqhhznrws.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gaqarodng.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gzhorjlqu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gimtfqmzn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbnvpdiug.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gljvxmivr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/ghlalgzdb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwqoovmhx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gacvjenpi.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gzdiqeupq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gsmisfmvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvtahuive.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gdujzoogu.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnssdiuce.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/guihxqfps.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/grnkbjvki.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/giltxksbo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gkqmfvkyv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gstflxrdk.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/ghiqjkiyy.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrgqtsu.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gwvmzeqyh.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvlfqxwqy.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gitongdpc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gthjvwumf.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gnwetxkfl.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gscuqmfkq.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gueemddkm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbugcsojn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdiacgdwo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gmtpytfgp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gnynwhigd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gnzanstap.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gihkqtoji.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggcideugu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ggndyrviu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gjuxjbmtk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gajeboums.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gidvezswo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdsgvnump.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gveqwdaiu.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gdhqktpct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gltywtyxk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxpackrpe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gmellsvuh.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gilpbueyz.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/glptpnncv.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gugqtoyfk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gegdawmwe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkvoohmzw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gcqqjpjxg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gilhziofa.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gunjrzcce.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gzstxtsls.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzbirwpnm.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gmnqrzogv.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gsolzdcpw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gdubgufrd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/geegqcvbj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/giluqvbfx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gihdcbaok.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gjronvzbo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gdwzxjmty.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gplobsjjh.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gmjknfixe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/ggqyhaxjl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gjhfjxpqo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmgxmpgqp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gwzlumrvt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gologmuhd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gkzoywwkv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gycuimmxv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/ggckkenpc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/geqphymdh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gsxprmwtl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gqgqckwhq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gxzcjhlzh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gbprdtglv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/guwvxkenf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gxrwehdxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gazkixsro.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gcohcykkx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcfihglnx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gnigntugo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gojysdfvn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gkkvxhbte.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gefskvwgs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/ghmlwnbqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gjfcfxzgx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gxhdzgeyj.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gvuklvxlg.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gtiepcxbx.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gmczwqicn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gdoygvtvh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gcilgefzs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gutcnyazu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/ghdxpldyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gwkinbwng.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gymvpatzt.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gxngkkxmy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gyhefcpvm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ghmpvltle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaykzaizs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gerflqecf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/goajvsebf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gnpcwqktv.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gofhglvzy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gucdiptjp.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gyvllhgtd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/goygnjcow.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gjzlgvmkp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/glatedfwk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grxpxmzli.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvbxxgdgd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjzwcoyxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gbdzefolt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gswcgcvdy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gaeugnoft.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ghgomlqrl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ggncqpurf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gzthtyxun.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gcjkcutwu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqansigux.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gamsbegrq.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gwlxtzlgg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/glgbhftsk.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gqfupztnb.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/ggasxcein.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gvgdpajve.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/ghqudflqo.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gzgfgyllr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggzfmyrhj.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gfnuxbtwy.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/givxlhgbg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghwhwmmym.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gnqwfvasy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gsnsusurt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gjtmtzgde.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghtjvbsiq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gktmqpphw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxusgtkgb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gjtipjkvb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ggkwxajox.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gwsbudkuf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gzpssyqtz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gahodgwxr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gplpieddp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gigeeokfv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/grlntujft.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/ghgwufqpv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gbegzwynk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gucdppalp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gytqdtsnt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghlgteqnp.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gmvrygbpj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gegizbwbi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbjzcmiab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gyrchdajo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqlqylnoq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gejrdybdd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gaemyhsga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggpedpjkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gxbnkzdoz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkebcvtcg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbkvmfzgd.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gzyfkddyj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gqdftyzma.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gqfpxqccg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gdlavchjs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gtklktdpd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gmviifxdg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/grtbysvti.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghcnzrkis.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gfjzlrats.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gtebotuhz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbttmlrvs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghzvqbvib.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gikqkpfhr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/grxkzjkaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gnrmolflx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gstaagnqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gekymqdht.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gksjpolns.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gxxydfwqw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gemzyecoa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gknzuzknf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghzditgvv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gyithuwyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/granpcgzh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gnpkwlkay.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gmzsmoavg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gdusfngit.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ganfgvrks.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gdozybrmj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjbwnzoas.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjxcklcat.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaxaynfag.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtozxzmnv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gahszclkg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gctwyubkd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grmgzrhcw.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/grbllzfmq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghrhuptxa.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmtgzngqv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqifsmtyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvumzmrnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmahmtxfz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkswxupvj.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/glnwhayca.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggmdtuvng.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gxztgkynt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gohnxvuwv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ggmotpghx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzpygtysr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/ggmnfzsrm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzcilrg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/goszknodg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gekzluoqp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/grpwoniiz.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gsimvtijw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gvavwyads.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gnexqmdmz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gkedxowvi.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/guehwopbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/grdhvawvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gbrgwaekt.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gellunlnn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkbjwuikc.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/grtinjpdu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyrsvzuxw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvnqrekuw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gcxtyhlws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gywzlhhsn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ghtnokmvy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gmoktbeeo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gglmukxca.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gedovyttq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/grplwxxmh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfxzrzgeg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfxsrdbhq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glqthidsc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gccndopei.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gbqjfzfvx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gafnglvnh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gykoasqmj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnjomybmk.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gaofupbyy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gikbuncys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggoiqmrba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmsifpofr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gfstcbzjx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gzqhsvwaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gjipatqsm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmojihiul.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gjzhllrum.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gzvqriocr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/ggjgezuoj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gtffrrmib.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/giaeuuhis.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gipiuyblz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/grumjxvte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gqoqdlbgh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gmzouziph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gspihtbgm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glyhdavgg.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gcvddyqik.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gncutlzmg.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gcztijdxi.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gvzfyxscf.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gzwhfwuwi.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/ggmtxrxoz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gnmipxgbe.sHtML


<!-- 参考信息 -->