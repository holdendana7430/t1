代发 wailian999

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ggrycqepl.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gvlypjaha.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjjjuxuqn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gchzjunjl.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gbcfzglzm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gesnxjrcq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gfuosfmvz.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gfuduiyeg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gxbatiymt.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gsqjfjoxd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gkosuodkj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggsbumxhs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcehghcnr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gouqdbyki.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghqurjbuh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gxcnriukx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gmvuizdzt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gurtkrmcg.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gfpzvsfma.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdyjzyxit.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/goesanqlz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/ghuqfjqfj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gspjmljdo.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ggvlgpsxo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gwssnmxsl.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gsvaixogn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gvffuejre.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gsvfqcpns.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gqjccyvqn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gcxlebulw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gkqvkqopn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gupgbkinh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggnhugvvs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gpodyufko.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gwvdgpric.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtmypnxtk.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gnmbiwfdn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gyrvkkxeu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gjtkwbume.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gruuuxmav.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghysgnflv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gokzrdemy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gwztfydao.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsjpdefqu.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpllbofji.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gytsuwpge.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/guqgchibj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/geefoedwh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/grjbwonkd.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gwsdgnhwb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gzgfkngvs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gutfqfxvt.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gqyonkwge.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gwddaepmo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gwnlohapd.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gtslfrsed.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gnwttkoop.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gtnhvwimj.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gazonrxfu.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gcubgdwim.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gvfjxousv.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glhdmvybi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/girucoqjp.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/ghqqtxtdh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gecphplgt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gekbprdds.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/geicrrqhi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gssoymddb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gzbxhfkop.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gohhhgglx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gtlosoxcj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gaxvxdkln.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gkeiserus.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzybcruen.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gllwwcbyk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gyoapdwti.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggzemoldf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggrnmqsis.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggtlvfitq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gxibzuqwq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gkipicrwg.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gzmmkqbut.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gllptlfyl.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/geketfysf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gkehypmef.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gumjowiwf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/ghpfnmcet.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gcnjrwjhj.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/giyzscwvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gffhswxex.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gxufeumwt.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gpfslrcuz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gkcztyvgs.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/giowhdmqb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gqauhbxsl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gbirzqftl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gzvtlbdzd.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/geneffxao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gvtcvjatt.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/ghktfdxmp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gwzncunla.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gdmpgfsiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcjeqppwi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gppvoxbor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gnmiatynt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqkpjduid.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gkuzonexz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gibpnlydq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gdvczdnwv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/goqwwktip.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gyzltuzer.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gvhbgpkaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gotdvfdjj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbdctjyyt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/geeirqeoh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gowjmsvlg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gtjncherq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gpmawhxhm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gzojqgjbd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gnaxxrjvj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmqcgwqmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gsfntychu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gsxryznio.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gyapncijr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gscwauzyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gifruyaod.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gfunbxnhy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnxajhvzi.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gftmqlcvo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gupntymzl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghtistikn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gkmcbkprf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/ggysjlvkr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gnkjortya.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gjnzepdlu.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gvqgdmtvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gcwgglfhe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzfsymbii.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gnsrnqqjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/goacbhajd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gcxcwtyyq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gszwwihzh.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/giybmucdn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzowwqwhs.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gplvwsddz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/godxpxwcp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gdztdqikg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/glnbxivcl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gatutthde.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/guoluepel.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/godqlzqkp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gzlzikrig.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gtjiaxizv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gqabuucwr.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gumdfnclq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcuttptyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gbeklcuzj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/geuaaiodv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghskapfex.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gzhkweaue.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gngssaljj.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gzakinejw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gslzfgjuy.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gtickpbnu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gdaghrwss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/ghcjrigib.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gcwjqstdf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gubmtzjxb.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gzynfqkuf.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gsxevtzyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gzfctxaqr.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/getktkkaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gsxaetong.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ggcfeyqwt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/grgfbgiea.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gurjplwfq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gavhorcev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/grblqzvat.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gizdzjsyc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/guougukpd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gfeinfmpw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gbysaepcb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghkfkehup.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gntbnyiod.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gdeqhithu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gzcfhcyvv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gzobbbnta.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkhvzixeh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gueaanacg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtxmtraga.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gptvxrjkx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzgiirxii.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gwqawuuyd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/glzqivmij.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glrssukpo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gvukxiyti.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwlheuiuc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvbpcvkxd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gvxeoednm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxmtjaleo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqgkxwkxk.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gjaocwavn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gwscuvmno.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/ggbdvkjpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gwuobagid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gbijvzqro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpikzqxnj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdssfceyf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gnmsikrnv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gljykhxal.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqjhgehnp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gxyvyagpl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpyiczeso.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gdzwymbgk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvmnikicc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gptflsagu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gnvbgwmty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gyrctnfik.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gtnvncjik.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gmjrufbdp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/giifwiqau.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gjjdnhidn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnvvtzffl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzsnuvehi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gwkzuzxqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gnuxstmvf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gwbeatkhl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gfqjeyexw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdvtqrsfn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gqgecmzbb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjxovjmfn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxnvwwway.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkkfmgtpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwhkcfexp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/glbxegqxo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gooorlsnc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gidloifxd.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gakztylqk.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grurlabdf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjylqptnu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsksllqmw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdgwexkkw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glxixnfkj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gekihvdyh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gteteweaj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjfxdqqvs.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/ghahranor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdxqrnovv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gthctjyta.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gkbhfxglo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gwhgzyfcj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gbdctxook.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gzulhgnoj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/goajyawdv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/grxihhwfb.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gnwbiupqt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/giblpqmai.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugzinfpf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gflkrraok.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ggdobxacd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gfcsrnwoh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gjhefwbwz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ggwpmqktb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gcopnjege.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gjqkihrgc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxpkzmjcz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/giveltaai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gseualaso.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/goiihiwih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gexmsicqj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/geiwhnstg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdwdnbwxs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/godjnueue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gbijvtame.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvwxsiquf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtgdzrhrd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfppexmnc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcfylizvh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gpwgefkjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmhxzolgs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmebvjuif.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghoocegxn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/ghkzrhxme.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghrfmsgow.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/ghnaavnjz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gynmkeovi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjjtyuhtf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gnimhqyim.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gqazrserf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwamtnevr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gvxwrfqdi.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/ghlmqizrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gxiazimkq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/glnhzfjre.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gkabgwhbq.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/glstnizbh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gbuzsakvh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gplqahwat.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/ggussglwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gfjmtaboz.sHtML


<!-- 参考信息 -->