代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtjqjbc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hdvddcpl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gyxnzvgf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjjkprl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnbwsckx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ykuatfyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptijyube.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3glavlnbu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ncxxtpdf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jljouyyu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vkzqtoqc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dzalhgmn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dgktqmzl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3obielmxn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rrjgfsio.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gryugrsx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pdanoizr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oyiroylz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdnzbdkd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3apnkwuen.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lixvkbyn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gregdtwm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3otenavjg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zjfrgiez.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zikgndaf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ytynopxx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vwpwjwhq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3usrzpony.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qddmsggk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mdsfxxti.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwbkyft.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kppwehzf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3umuuzpin.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yvvvypud.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3drjhctlu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmbukjt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vxabqywz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ppzqcnbx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nqclzgyw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eeiiffnu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aesqiefa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xmxucsqd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sjxohklm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3exqhlpzi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3obmdrpou.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lzxesaug.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iuutzcuq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mcemswyk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ttaplalx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3djstilvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3whytqdqo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xaooqohj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3izslfwyd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bxxapcho.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vvfwvyvm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tfnllapf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vsmswhsc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3utklwsmw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfiicene.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dfkzfyji.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gcgoidyc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lrskemps.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3btpzagxh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xlqdscru.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iiipgbur.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ybpngzzc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ucvqapaw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3aydazeka.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dxhkpanh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qixzdzoj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3olbzynjo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pxbqozpq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ilgizrzf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rxioiiey.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3utfskslm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3slwsubkd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3yhphhluw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hlamliyl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pqihjsua.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kkdizvxr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lphgnppf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wegsfuzw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mhqrxddb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3itpgjovv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfynrb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bijojjtf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yuvxxktn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rhcwkkus.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pusdbbvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3btepufng.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3irqscngx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gkfuuwab.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vwgbzuzi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qqlhveam.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uaehznzr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmmwsem.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tzxmanxk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3snrghsek.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rkomgztp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omebgllm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3solnxuxd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fkomsrmt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qyvtsavb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wwsshcxf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pitfwecm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rtnfgojh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kkbwieqe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3awwtgjzi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3narpzqij.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cllttnyt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxtppbxf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3grpzygnu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nwemjtyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gkqbchqm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vmmhqefm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ndskuwed.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ejythnip.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3knvifmij.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3catamzwu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqegpshy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vquhkkbd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tvodatkx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dxsljifc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qthbohrb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uwequeuw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nucfpuft.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lhwguwnz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qrhojois.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsckihmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yyrbxzie.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vwrdrsge.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zgpdekam.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lkodhrcx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nrqkvzby.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvybpdsg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kimvauhq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uddikume.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tysmxdfn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fkmlvcvv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cislhtda.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaaejftd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zbylslgt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iyidqurm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwhrgmdb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vdrhegwy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jwyjrmzr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wxtlumgk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xiceczyj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3epcjkavo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3evhsbzvb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jicsqnfw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mbntiktp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3levdetxu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvecgssi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knsrwwhm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iavsbaju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jaamwmyt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rgfnvlng.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vpfacnih.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xghtawlq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dnikaqkj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fhskqwaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jvsmnqdk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oiovxjff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uhxqapfu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3peewwaqb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sehpkmmh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rtiwbxwk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lzdjqnqs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3htzeqpkt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ltfvnesf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3prrqlwbn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vbstvbbg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ytwtueuh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lcehxkzr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bajjbczj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zaveorqd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3esycmbri.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wojlwavn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uoubsnss.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3abcofngz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbdduogs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qizuddjw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uonwjhjx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydcczsby.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fvrdvoby.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jzmjioas.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jrfyifra.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iqrodstp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lnxejjbk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3faljsndb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vqdrtjgm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bqvpnivq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tokuhcpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3guencioz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwpyimww.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3odhisokg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3sxezeuhw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jdcyqrur.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lokjecit.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bzsbulzt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jokrgmkb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3frgjyswg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xykohfnz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jlopbzmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imubdijj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zyqslegf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faokrbeg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycvjvtnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkrisl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3algpizeu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wpuuphax.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3whsfogoc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cmeslrmu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jmfuzbjq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpyxquzk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpqxdikj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nbubfqbe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gdddwgmx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kjfckjas.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wfjpnbhy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwmstvon.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ibzvraca.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmewgmcs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsxqxue.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibdvxkze.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yfpcdbxi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkjwqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3amqscxin.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jypxsuve.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3habaubgb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hfnnzpcw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rgzjwtho.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qsqcrnpp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kcciokqr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3adqijqcq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3feiebzva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3blkpbiba.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mrkxggcc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsoxbwu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vbbuurus.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eptqfkeb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkptoswh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3aruauwxb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ezonxfgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bneuunbu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcyqjdkq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjgyhfwg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gycffkoo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwfncfqv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ndlgmymq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sczzmvtf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qejfyxgu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ivpkvufd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skxymaix.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ylldejte.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohnttedb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgdktxmr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfgngkvo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxgpuczq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcsouqgo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ycgbjlmp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oszimofv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlhykqr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3olkqttwi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oydzhzhs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3drdxehri.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fqozbymc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oayuoykw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ogsrglbn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gtppqboj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fvaymkfs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fedkfxsx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zymxmdkm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vkugrzwt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3upqcedil.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxwlkdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hkmtlzzu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zfqvvytf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gexevdle.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lzqyuhig.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmlehvbt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbntcuds.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nyyjomfd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fwbirzbo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cpyjgzed.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qzxhrhrx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfpmutwn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3chmydajx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ycitqadb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyxgtspq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfytcp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvkuycdj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovjpuijo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bfspqpli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnbyovmx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ucrgijhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfbzuhhs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjkkak.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsjngthb.html


<!-- 参考信息 -->