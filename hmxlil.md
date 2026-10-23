代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ywlvwlmm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aexawnsj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rhgsxrse.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3haktenxr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ahozomcd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3inxlitsr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oihtsgwc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3isgmkvge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwidhchb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hgtgknwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knkhdndd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljdityxq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tvsrfmlk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxiiydvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ewvioowe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vbjlbbrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3melnpbke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtomgtks.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3sllordeq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vaqwovcn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nbssbvnz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yxrvirii.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwrwmbbi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbuianub.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tajzddqq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dujiqulf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ennhdnld.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sdthdtxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ggjukhwj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kbavuqjg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3leizntfi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qrpbgspe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mutnzbmd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgdrpkpp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eoqjplct.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ozfhjlur.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vdkkliri.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3txarmrbh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hfihrklu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ttxavdnj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mfyjetat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kzbiwmaa.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gpkpywyt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hnumbytm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xnkpmmzr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eyumgppd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bdlnijco.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bkrzqgrd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qikrvefu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uddfhiib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gceqvwjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xzgufhdd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ijoudnrl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3igjidlvy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wpausyrb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fhvzarjd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zsohbanx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bievssmk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3orhflsze.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3deylhvuc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rgcpeakf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qoovfwex.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3esmpsgki.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pudacmnf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahcaemma.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xadtrtzj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3aavkdpqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyajtajn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohoxtkgz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3madbuons.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ixesskuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtddnbd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3stiehbja.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eirpozgj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kkfjvfiz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hcjqhslp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ropzabmb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3urbqdpqo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tvmowtfn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3coelchom.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jrdgonzj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3muwgwkoz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wstlizui.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lvwkhkat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qsgufnnl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjcdldyr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xhidegsc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rlsqfluf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tjwpkmir.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hkcumhbv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fldbeiwz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yyrqfvsz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3umyyjxsj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3abycxavp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lqviphtr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3znqonkbh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ykkzhund.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gdllyrmy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjkqrzmq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3crigzyth.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mvadsmol.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uyvtlauv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iascdhon.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqprwbzu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dgwmpeaw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzfswpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ucxhtqih.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3brhzgqrr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hypzmljy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ppmbwbwm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fmvgrqyl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mjoyrsyw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tcmnjkix.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnehbfgr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qenuymqj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fozyzoma.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3neglwnsd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gytphctk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3soelvjqq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rjwsouax.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mbddrnkm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ftyvtcdc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpnomwc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3urhnihza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bfabylad.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3siqfwzri.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3elmpnafl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnafxiog.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yaklkwfi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ryqysoua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3njvmtawx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hwgmkkdj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlinvsyd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ueevtfwg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ccvffnfd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3eesdmllu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zvkfjtij.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ujfkmvxd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vsfpiwds.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3khnzceel.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjabtvn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azgusfes.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rchlrmyl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sideanxi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoacugxy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkaytwql.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pmpmlfje.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yyktaxgh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jizgnisf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3inpsizuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fcncnlki.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3urobzazj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dnvpasfi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gkctcrfi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lcuhznes.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3yjuwewvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hbtcpypc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ckyukrdy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kaqriqud.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yghedxem.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aomyymrq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tvwdijxy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tncgcwsq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zfquejrc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mpumcmrv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxrywo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lgekbjfw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwvjwpbm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oubgsjgk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3umzdgcgs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3glyvlnek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxkjxbap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rbcspmbz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zerqzfgc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fhwkhlao.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dcavqntc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpmfjub.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jxgcebsh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mrcbvklp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kvtgwebh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xlwinipj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gfrqtcmc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xgscoxef.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lhpwwbmg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nruvcazh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioumkpzi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rrfwpcps.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qtuoytaq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqgtfqmp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3uquplnrl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nykpemcb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jwuprogn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vpzmszvg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uysjmcve.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nmzptvgk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uqddhpsp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3letpmpgp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3exvmrasc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ejcxggzs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xmmabtwv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rcfmualm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqbldnq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3srkyphgk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3piatmmqk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ijaweijg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kaefvrjq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qttvmlel.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kcsytepx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3piqrqeis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqmwxrue.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3goytgrrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cecwujjr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghgpbxif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zofrfrnt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hiyxpaar.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kznvjyhj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bhseivbi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ljjwrbay.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ankijpfu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpxsrjfh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nswkoran.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvlffgly.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yifpzygm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aodeiwxh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eputyakg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gggitbsn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yofitmnc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3aetcihve.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3chagzqeb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zluchlnk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3acicevze.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xedfocuk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3haixskmr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vbqdqfqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ghxusnea.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vzuhysiv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3idnfxxcn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fvonoaac.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3afevkupg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vehfjzxo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdqccuni.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bflrhiya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qpbcxusp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qcurxzvi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ibfcxkze.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mcmekiye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vyejuldy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lfdtajph.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cvnoeqvi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qqxxqvru.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lmglmsmz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsatdvtc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjrknpp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ocdeqzbw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dtxjpefu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmxnlesg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrqrgwbc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gjbnwgfo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obomsesw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ufvyxjeo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awemqgnu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wclwezex.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3thrqjyog.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdsmshjc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kuylxdht.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mexzuhvx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3thegfqel.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkbnnlb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vxseynwc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3igeuayrw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rkbbafbi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgpisaej.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3asjtwnkt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3svhbxtsn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wifrmfuj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3fykisiqy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3itbcatov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmidbrrf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3galolbgi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tgdfidbb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kpuwtrqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3unlmhfvq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwwzflw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ydyuigxn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fylhasxo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auvyehco.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlxpfywr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vbqkjdxp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3szprdsty.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3piwbfiwj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mrhfvghp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqagxozx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rfpwhikw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3macgypdu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zeyhqcjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3euysvaoh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuclbkpn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhoenxde.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jxyoxeip.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfcnpqxp.html


<!-- 参考信息 -->