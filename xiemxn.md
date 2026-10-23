代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cxnymxib.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dpwkownn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mkmkuoss.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3swiratlm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xuuwaxyk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nhtkfyru.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eaprcaay.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cteksszc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfbtkkav.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3opvcdypx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vblfchug.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fuyoxhxs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mjhrhzai.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qbghnilm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3airduhqm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xaqqmbjo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dlbikrvn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ueuiplmr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3khmwlnvr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iclxxken.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3iykdcctb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ewjstlkj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xszvppwi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3obojrgmq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zkhzmryg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3unaumgkr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lniqaqvg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ncpyflff.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tmqzqixz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zkfidddb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tyocqubu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rqslhvvo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxshtja.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rpiupyfr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fnikbuqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wlgidygp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3utewkppm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nceydmwj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dgkdnpif.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nynecwwh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3petkymmx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mblwjtwd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hifjcfmu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fozfivmq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lofzpjiw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhnlsrvc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zkgmmxmf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hvyakbmy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hxxwpodj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fjgjxiiq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3coapgijt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vibhllwh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rnqkpzvj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wpeuavju.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pbbymaej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bnbmshnb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3idugjynf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebfwmztv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqajxjis.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vqpjiezi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ievtavyd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vaaupbbo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nbqthkuu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dvxncohq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zhshfpxz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3koubgaqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ikvsmdnv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aqndhqdh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkvnpkln.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3iojhbwwm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fnsftxgz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ximqfxow.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rqnexopt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rtmzvwzt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jqajxesj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3djdxurcd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3glzgftcb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ddamjvdh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xepxcyaa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzepqul.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gdzbxitu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwasjpou.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kwebehie.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qdrqxcon.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oufsghxu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pgrcfqhb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3myyhzcyb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ypvbydgf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3migtxjnj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xuphemtk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gnjxdara.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gdtassuk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lrooxqpy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ctzuegkl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwocpkv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uziynguv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lnzmoglu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pffcuyzs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cajxwemg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cqtfpumx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rhqjdlrs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3aprrnisw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dxxuponz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hteizjaw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3djfolbze.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ipdwdqvb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dyosxqnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rcvduviy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mgotwigh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hroprbco.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bebccexz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dknktcgj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sscfahgu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ypugvzew.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdlqfeyx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gsfiuxmd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ftsluxjb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lqwlstcc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wbklpbcn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hfjpjzmx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xlkkrkfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcqsjdxi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdvojnv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydbaskhw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hthnjcfi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lrwwtewg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3chxcohvw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zroxqjdi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mfnypexz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ywsvdncl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qvqdaszt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lguawfne.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dxfrtdfx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mxqsjkin.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3acblmdpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mbaftkmx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvlxzvb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ylzdrsoo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzguvly.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zzmclrmk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prwogvep.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ydjlaqao.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pbamepov.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eufpacsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dygeqwfj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbxjjsq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3phvnnhtd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ipbvqqzh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ykhuqrww.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3osnjrzes.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fyjewbza.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3izvbhacp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kyrzdirg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cvmndjvw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3oafdgfkd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vgktkerk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wwytofsh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3isttmdyv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cqmwlbus.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wweflwei.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jcejwyfn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yufsgndq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3otvwuztj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xhcxnhvd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3acytkohn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oigyomrq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mmxzzwlv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ktjgwoku.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zjgwhsdf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3solqqgcj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxtvhyz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gnepmnzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hexqxpbq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xvkvjfur.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3tlzoxjsm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ygidksyz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ttwsbsxl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oieqwlqp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzdwsnhs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3calzbpyz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3axdacdpq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3isxpnqsa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dknkevwj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zkozimjm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zkaojblx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ndcqplmm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbmogv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjzpkkrv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnmdpdfi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cllhrzur.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpfkandw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bllcglqy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yxkjqlug.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yucmkgqu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bpptfpqf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ehqngcat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mivkxzic.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tlvlwjjo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ayrgyhfc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ovircfoj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3aiyxhktl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lypfcpsx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrohvhrs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jgznferk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kxadzccb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nzqeprck.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rxdkrdpd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ngxpkqqa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vpwlmugr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yduojfiy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3klkakhhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcihhtru.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljcrlvfn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xivkkmxa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3buvgbtyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pnpuhoep.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nywwkijk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfspgdyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ceftzbdc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vccserum.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ishsghtu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jndfgsdv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rfcvxhuu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3btoinben.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ywldzulz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymqltyau.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lyjmfymg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wmfofsde.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wtkyycjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3waijqnry.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tpusnkza.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fgtpbfat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qvujcuag.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kbmqjdib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3algrsabb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nqrjesdp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3itvjtxpn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3mwgrqhzj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mquiavdj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kywjjuoq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dvpqmktk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ackzambg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gfiucpzm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ixldpldl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yxfgclwg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3amgxieae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rpqvtiwf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eblfotns.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jfcawhmt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qxjlgnyl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iubybbrr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpnxxxyh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsedcavm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eunjqvkt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wgystdyj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhfocykw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpasin.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvrmjnjf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmcqhprk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udaiwmzb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izaghcez.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3primpgrq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lyllnqzg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3doskjzqp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyqqaawz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aicgebfs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oimelkvf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wicsafwm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uuixejhj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kseahcte.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uevhxuwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vaiwvsib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3avxtzgov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pmsdtqjm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ybgycbnr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rybaybdy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fopmkvaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jgnukdhp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hujiqtii.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zuluxgdm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yvckstwm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nscjifah.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3metujuid.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zoqemmgm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bpariwrd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpsxfplk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rktslcxg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jbpppoqu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cbdhuzwz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqnivqai.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pvqsgtxi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxyorufk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fcpbfpfj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gsczjtuc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnrxkkhq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qfpldfnz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qumejobt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grrcszad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lfkelqxt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efjydhkp.html


<!-- 参考信息 -->