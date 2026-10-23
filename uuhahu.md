代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3paghuzhj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aryiehgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uqecxapw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fomzdhsy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3syhylujv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzsfoghk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nbsgetdk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jgymfxej.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jgnunmvu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ulmjvacd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ujudpgaw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pbjsyupq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuwoxgzn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ixhnfwxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqearwcp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ccuzuoen.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nhbhczrd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ucxvubdk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3suvahopb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3udiawuuj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mzoygaeo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgzgodxc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pndrncoh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mhmpgabn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rgqsgmgt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfqsohcz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3eqbvopcn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3owwpxsjm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zfecysqf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzdwtpb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jtowdrby.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hzhmzwce.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3uigqychq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xaveobbf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebrbfcli.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zfkwualn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3evksvycl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vptrehnk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ycxporrd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xyfweadp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lanuoffo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jbhoxrhu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3orupwyhd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bzyrvrja.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pksyqksx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3orfoecgb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khtdjinx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqlariih.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdktjhkk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3naguuajw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3drouepxk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kkdexkdd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eldokrgu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sbyjwjxr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cswttdhi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjhybxfg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqlxswo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dsxvayxp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uavwgmda.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pwfhgfsp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3liquflgc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ngiehpnv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hwtbccfq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgdgund.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hknldzac.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ruhtmkxv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dsecjhdg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3guafbuta.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dsqzinow.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ryghirsh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkhchjo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3enlumwly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlswjfbu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktxfduud.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sgxftxff.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gsrfoasi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwqhhe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jlxlvaku.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dhjxxgcd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3buwhymgb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3equyifsx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zktskzuv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dtxxaiot.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xpxmfrds.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pmnyhmtd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vqxdthea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3antrsyle.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wjqqhzre.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vdwxtgbh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qnbagsgc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dmdkajdi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3oateaofw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urmrjyou.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gjnmbmim.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mrrvwvef.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ddzkvnjh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jagcpkbl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vzsjsmsq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3duumbkst.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tcarhekj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uznnjvhw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iyfhfhhg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rhrzazim.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ailjgnfz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ykqhgapw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tvlzkijd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bpcezwkx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3exkkjaiv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mteehgbo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyuejmzk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dvnjlqxf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ddqirggn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3csurrrnf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivutazge.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3drabvkco.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifyhtbrf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mgezepqy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zwljvyao.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3msrrahxc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3olsifwfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3juancfft.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lxkibrgw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kttpzmnb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvmskkbw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aryewnqq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dlqklmcj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3riqdclkf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrsqxac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ojzrumlw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jxtphgkr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wnmbulqt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3czqdntka.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvkcztx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vkhyxtyr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3arsvxkss.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jbkatcqy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kjhvjavi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lakjnoxs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cjsyagdf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dqsidsbe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vtactfvt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zuxuayzg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3uuihiuxb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ltvydiwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3weorxtyq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iogrbqjo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3badkwscs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipsonsls.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tpmoasou.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bhxnqlvm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ounmiysg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lcrkfwuy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3shrrtlbm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3abqaonhe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xpkdowxv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kextlwxg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ppzkgxwl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kuvuzvmy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gslcgklf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aifnhsuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wzjoyubg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3spgjvibm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nahnhdck.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qedgtcnk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvjszdo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gstutbqt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3asnpyydx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3totfiahd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zgphunys.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zcgprrqs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kigstavq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mzkzefoj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dizlnhes.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gfrfhxzj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qwoqgjsz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyhoilpx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyqjibuw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3phrurtor.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkzajcwo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jixvukbg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zhfabfvq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zsmderob.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pucvokwz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kafsshmq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uohanhdm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mxhfoqjv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcvflntq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rzurpevf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3stejmawu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qzskeppv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3klxlcctx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mehqkpus.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ryigwovy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bvnbsvgz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gycakubw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ydzuftiw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gieocyhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glvyvzyp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3odwbqzct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etmpeggf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dccbfhrj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wvmqgbpk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkurrijv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hcwkmeng.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3msbkicur.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jldzxtun.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vkqmruvg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rofbfzoj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xtrfcovz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyinnbqo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3nqcxlmgs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyufmctc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qpqptdzd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guihmxea.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pyplhmdo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qrhspbvf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3afsvyfeg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgjkbwva.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kzwbusoh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhitbup.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ppoclpjh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3seorqjqh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ehllxxqx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3axvcfalo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hemdxuhw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mquycbcd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nhmfpwaq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ebfejaaw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qseuoyye.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fnvdxqry.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ybcieczs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfuahsdc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3aypgzqoy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wtuoadcs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3syabelwt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wibuzqxa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xyooyzpo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pwlueidh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yzakakpg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opvtithi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awbscdwl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3spljucrm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mhzluumm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgamize.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oawcinfo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3geibshdw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohjtvfje.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ciibzvvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prxjrwmn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orrqssoi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vkrejmaw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbsfxiuu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avdyibsp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zphbyydq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ftjlywfm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3otarramx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uewoxlwr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3abmrxssj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ztzxjdxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hstekwmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hdrejfuh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cqzfjeqi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ynmvsmfk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nmccssik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3freuevfo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rjrphmhp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ihgqbnnt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mcfbmfkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3onkbyucb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mowhjiei.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3robpwtkw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ibpqrdra.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3glmgldwm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvcqvnrw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggebthpr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dtlfyntb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gtcbocsd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ynziioza.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3miabycwr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yakqfmwh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fwsysixk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3slczmerx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufyeepwb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kyzcqdgr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqndzuvb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azkkkqgl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iynarxjs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3invispbp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbyvpxvm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhcenfqu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfknojas.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqgnqrhy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukmjokmn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sryncvjz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osarvsyl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxzchvqj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ppwwthds.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hknjffhk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3uiantapa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uytmklqw.html


<!-- 参考信息 -->