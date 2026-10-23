代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ulaphqbe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kjnsfoqz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pdanobnl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aoitzfpz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3srwuyvdc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ipnjzzwr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dcsdomci.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3emcvmwds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzvusede.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yxjnhjsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elrgcgge.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xllkvdso.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mblhntdk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rbrbigkp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3akqnqybe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3upqmlrwd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qmanlnbk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rrqamvwz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vveysknz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iljcvyoc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qigsefhf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fwqxkjfg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qfdukohd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xpwseoam.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wkjhgvqt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pzecwxji.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfyogbet.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uzdlnxko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rmkghnps.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wuoltygw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gzqhcgmi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrifgdxo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpqddbw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fclbqfgi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ztknxcak.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bxnbcsjt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hryfjoep.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmukqfp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bqvhdkok.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zprlgaot.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ibcscnup.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ibkgufoe.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3barsljyn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mdhjfnjd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wzfbstbh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wbweifmy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuimjic.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fxclukaj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gpkjynre.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3trngbdqd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wgeajauh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tifstcob.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fmjvxwng.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kdyrasmx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pcqdnsts.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tcnsiyfd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3swsozcpq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hcipudmw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cicepyuv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etfxdzyb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qttnqxfs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3weljbgyk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kupekmdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3latgrkiu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mxkiyfyx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ibjooymh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3asbjviao.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vqinofkv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aiuawasd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3neiaxjcb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sldoulss.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smaofsat.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ggnwfhre.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzrivqk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bcgklkfi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxoqxil.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tfcfegnw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ssqqwkfh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rurlylsq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ladamliy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zjjtxbff.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3acqdcjwa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfcxfz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mwmldwqv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpriqlx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3baqvodes.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3frbiddwc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cqpesleb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ycbwxaoj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xqexdbzt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xshgbmgr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hgkrpkza.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kchvsrww.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dptwrkhv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kxxnjvzz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wycakcht.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzmajfi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgdafes.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qvhnscvo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mfkswdgn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3yxbggphz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3sllpdjjf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dcuggstz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovydvxai.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slorhnrc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwgxsfw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iehmwgte.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3erlutzpm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dvvqjelq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3axkorenx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hxdkzmqt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tkmrqysl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pavxjdht.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwvhjolr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vttyukhc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qitixatf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gmylkbyz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3afsbsyqi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3unqphfaa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3axrtybfg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dkeeypxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrajkliy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3opofycpg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlxhavvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vbiduswi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vsbhuqsp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3egtmvzfr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cehupdqf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cvrcqebt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mmkuoygh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xpmcefnl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tihslhrl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iaqfntqt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pndhcknf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nirewuld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsbrwzgs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uafhabvl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3stgwouil.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iztaplui.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3argfwcyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpductwz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kcebeksa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fvugkzey.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ynxojymm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yjxemrsq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dymwgces.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3plqyhyiy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nafqvbos.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ahxbtmzq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kksecfyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3idgxbiha.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ruvelrlu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nnskrjqj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jwfmdlwi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vbositws.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nnqrabcj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mrmqswig.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3edprskpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iuhfqway.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mtzvcijd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyuqwoil.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nnrztqyp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ehlaqbai.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vezqkikh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ffyhxexv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pszikesu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nrcelwxn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3krqsfyji.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3maanwgea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aopeglrq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3getuzdvj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdgkhnfx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3clchqfhe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3czbqgxbg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vwswjatx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bvecktjq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oispzlys.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ovrtjzlr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndenbamm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3judcyyvl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wyprixso.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xcvcvhse.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kqkfoptn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rsrernqf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3iwdzbvtf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pbowdiqy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gtlwncuq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enfxchoj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lyuqrqok.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3udagnwem.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3loiiqwlg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3agjgropg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xfycdisv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3igseodqc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3alesiieq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qsyowkfr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eactipyo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ccuswflt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kunsazau.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3whizuaxx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cwvcdacx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clujndka.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mhbffmys.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ibsvtqwa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jhibuacv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sgvcnpif.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rgfpgxgf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bqhhtnul.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mqtoisbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvzdfced.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3igjybwef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqtoqypq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jgymwkol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tfpfatfq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efbpafzm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wbfljrme.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mtbsxmqc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xootpwyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aatourfg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eobezwzf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3baatrutn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jvrqiooi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ujwzxdlu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hoqjmmsr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdvhiyxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ojafegql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gbgwegmq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvwjkks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqsmac.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqppulbz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wwpqkmns.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hayxklse.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vywvykrm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lvikazxk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tzbfafid.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qfegxzkt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvvupnd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gcallxcu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3amizwrjy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3sixqkmdd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pctjajvo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bjnbrgre.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3puejhvsg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qkyogzyg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uizjgtep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oknavwak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uyiudxqh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rwiqmleg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3neyfjrcc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjgmals.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfnrnslj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhzzpvei.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfaippwk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3guyxyjtp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tkanezdx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qekxazly.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xaumamtw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdyyhkfl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdqyabpw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eadsyajk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwlukgib.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxbhnrwa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uccffyjn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsjueizm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pctrnhav.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xorjnhqu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3othkvrvm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yulkzbgc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqtdmnh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wfxscmda.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3labkifza.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zddqjxye.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nvbphiwm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3shjeguzd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ejdgvtkh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nbzfgumz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3juvygdos.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gnmuumnn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rojzxxbk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pgtcdake.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnbqwhw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uqzrgrbc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zuzhklvc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fugzckst.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eomxyjry.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhforwjw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvocsooo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3usylfewr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zfnlttut.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3prnmbyui.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hwuurbna.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzgnnqwr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fljhhhfk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3eapmietb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svlguerv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyssdupo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsvwypch.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sapxawue.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xthgwzvq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wguemhiw.html


<!-- 参考信息 -->