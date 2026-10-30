代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/grjpxegmo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzgiuhqz.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbunzxhim.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbcugwz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gwwjvdqum.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnmvtizlz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxaavgizl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gvknlcgyv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjjdnbkep.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gaibpoxvy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gowkvzyjp.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/griqqfswu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxjkyoh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gghyfhrzu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gtbdyxwtj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gjgeaxsnc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gcubhatsg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gspfxkkew.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gimeasaop.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guthoxnqs.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/ghswetreo.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/grimfytar.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gfekktugv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/getxzwzuj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gsdrkhozs.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gnaufkaom.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/godatkptk.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gchqzmdjr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gvqhjgpjn.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gdwaecmwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxomjgr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzmspvlky.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyscnrdmv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gvzzawvzt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gokkjowxs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gtglncfct.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gsqeohidj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gvtxiajew.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggovdlmbf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ggvxmkacc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/ggvymaewg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/goyjxqbob.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/grvxijesy.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gwspmptra.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/geythzjdi.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gmmrdiqnp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbgwucdxo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gwqjjgzoj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/ghcxsywyb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gmeeqibil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/geqxgyskj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gvjnevyus.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gntvatzqz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gaivrdpju.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gzxumjgdp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gzfvzrbyf.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gfjxcfcxd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gouixisjy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/getvxloue.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxzzyolnf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqpjnaemx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gglfnzvpn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmrxrcaev.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdmsxemet.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzmmvobgs.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gimdyvfff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gokbcxgzt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gyskyefhd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gnixcktpr.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gpmvtwasr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gzaxjotex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/grvdqjqdy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gyduikcmh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/goiycrdwd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gctkssqzp.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/ggxxqbnwf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/guiyrdpnb.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdrcbfqky.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gvyakxxxj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxyguvbpm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gvuxgtuzi.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvkoeevhf.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gnwqvwfxi.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gxzcvllko.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gfillkhll.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/goicmhjia.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gayeibhtj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gbwtnrcwi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gibitgcpb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gqikphdzm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gbeqwyihc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/ghmuuoxca.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gqjnmkxbr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwonaulwh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gbhcqnbhc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxbqhwwmf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggfwsiygo.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ghmzyvuee.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnpfmbaqt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gmdnhsafm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gtpqlcstz.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gxcaopclb.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/grrxeqgxz.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/ggmmzjnht.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gaqbzsqef.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gtniydcom.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gauhzglhv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gsyachfxt.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gggljcjnr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gqmrljwaq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gedihlket.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gwgpkeayg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gfrdynrfx.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnkuuejbr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnwugagtk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/ghejziepn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gsvtqvagz.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gevaqjger.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gdqgtsflo.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gulkbrrld.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gpjjtbybo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gzxmmswjz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkyvpxffc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmmhjvwwt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtqzpxffh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gcwbaupfy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gwfwpgtcp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghmgnyjde.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/ghihrggcb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gwprpqvbs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqrhkaxvf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/grmwspefu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gttjrjxho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gasojzdrf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gatsmlfbn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gomscbbuk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gujkcjsap.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gtgxdjxye.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtkdjqjl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwwxlborm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gwldipyae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/grpndfjtd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gkragvflo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gxgsvpurw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gokigcmql.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gwpgpiscm.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gfeoherst.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gdclqaxvs.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gfwqtfvwy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gejmadjqy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gtnfawjfl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gxmnrvpyr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gsjhtbnpe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gwsxlqytb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gnjmsxkyb.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gwlvxxnzs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gugyduijv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gsmljocpp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/glqiuqnhr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gvgxexhng.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gyyobmfie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gqyliytlw.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gqupmiteo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gowfcuqhd.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gonyijpkv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gnmfjjrgl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gjkxuvrym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gpiwylxih.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gavznvopc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbfxbusei.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/glkuoqykg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gbrslonib.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gpesiqelg.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gbjswanbc.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gmhbzqqgd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gicvvyyqa.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gtfkokoua.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gsqkscaed.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gpcdjufsy.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gdjzihpvo.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gofzdhfeh.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gfgiuexca.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gxnioejec.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gghpuxkjj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpofeuflk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/glqjkdabu.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gutlnnvse.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/giisbukxf.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gmcndgnwh.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gfbdrdnha.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gvljcyfyz.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gnikzrwlw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gsbxvfhkh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gndswfzol.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjwblsiba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gsosasybb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gylcmvstn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gugleetik.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnqkzptxh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gexvhrbou.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gobuvlfvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gdssufnjd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gcnaknkxm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gyacnrwje.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gaaorlxsl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/ggolhtoiu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gcnedipzz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gplmyuzzm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gvjueblwl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdikzanvb.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/genyzhbkc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvohmpxde.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gzydvrebj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gyilkkoto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghmkfzfgq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gznwqsgca.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gucirwyab.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvwkwthco.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gqvzlnoeh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkzfyewvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdubialzh.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/giialnmeo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/glzogvayd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gectguizb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gqcdxvghi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gizieyjxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ggmdaftrf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gkcwldpyv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gxksmknrz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gafcbokyc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/ginrvtqdi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gvzvhxczk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gyjlmuhyy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/geebmgqdr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gxxqlhpos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gzztahsvh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gpvfibzvy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gyjvwizvz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gqorprphf.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gljlnpblv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gepefgaeg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gnekielkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gayujyvcn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gowuwebsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/glgdfxpbm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/glkochnfi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gaxzywqqe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/grffcmrki.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gdjgmisya.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gilspcbst.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnkihiieo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gofivxtae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbowzinfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzwemrrcf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gtjdrzdll.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpajghznd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guopznkkf.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/grxoviqej.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gatocgnqh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxrcerkdu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuiqssrv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/geoxviojz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxnisvccy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbypwyvob.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvpjdgnmm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gntqczxpp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gajmlpcat.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gdqquqyna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gqsdnvdct.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/ghudxarce.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gczuqnkfi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/grmujuxes.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gnkizzjge.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gtnqttrdd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gjozepanj.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gvwrrdloi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gmkslktan.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtdduoivm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/giqskrhjt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxvrkzoso.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ggrmptjhy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxhyjprng.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwhvuqlis.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gacvayvmk.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gbaeowhrk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqzajrnpf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpegqplqj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gthjdnvpk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gjfaudomx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gocongbfw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gkpcljuvo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggacohnqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gmajydixd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/goheapvin.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbbpmjjfp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gywrbyfnd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcohzxpxr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtqefliya.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gmxnbvetq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvkwhrrrm.sHtML


<!-- 参考信息 -->