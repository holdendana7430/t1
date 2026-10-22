代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ezdrimqz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2erglkvua.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tosjujcn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvegteio.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvjrajwe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qxczhlyx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tmrdhipl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxudyuvg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tmroognh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2synhlqki.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2buxwxuho.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lavnyhqo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqlufef.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2krhbnuyo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfhmnkw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gwwbfgzb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vqsrngif.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bejlenoy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2llcfxfox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sqqvmrun.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qjsthuop.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iepqxrgq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2geesmrsc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pzswseow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jhnknxfl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yqfbriga.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yefenpzr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eemwdghl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2abcnrqvw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2pfscrwzp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ktntrlmi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mnktvier.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdvviqn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2srimvfbs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qefudzyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ipmtmigj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mxnqfion.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2asroyyfn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fwmkeltb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2slfuvinw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2galzhhzd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uvayfjup.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rykywuvb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rxlprceo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ggjjyoko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgeqttqf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2anqaexpq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tzzrpznq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cqodszxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uotltrfq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dizbsedf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mmmsgjcv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rlvcadyq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vgulzmmz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xvtsximt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jrmbaosv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cyivrrwu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2iqzgdyox.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2igcdacko.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bbxaclbo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2slmbioag.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yeppafzx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iutbwnnq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwgqedf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2swcpafmc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jdtozouk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fxwtqsmm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2knbqonkw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wsarqkce.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mbywkzue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rlxgxtfq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2usqeehny.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nxwxnawr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxbpcgnt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2untcmcez.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2toioldyj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2woqukfep.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cjuywxtf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sbklwvpi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zpvegysp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fvjuqwxc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wrhpgcxr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cdfqeauv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tmpitdez.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vscibhtd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sskkekuv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzpnijaa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eeqtqhxz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gzvuhwhm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tavaakzl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sxguinwm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lvksdooe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zfofdywy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bdepwczb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzubdctk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2alwpuwvx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uohcveft.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mlqwqrkl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hclmkbmp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kcuspgao.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2euslwisv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bcixepnw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nldmkatk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pggvzvtz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uifbdhfs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eqpgxwad.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nvzzjnyp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymuietdp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2djbfuino.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mqoslvhi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lfitkoll.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjhcacq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jepdxhyi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vgibxzgi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yuxiijub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldfzhhlg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qeqpqgij.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2khkwzmzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pllnbujw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2btqnwnre.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wxuivfpk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2atigrqsp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2osnvbqhj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jynkpiji.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lzzjjpyl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jfvfeqlb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsbamna.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ubiwukup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2degxwwew.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pwcoriyn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2guynuqdm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fzbsppua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uvswbakt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uoudyzjj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bkuigevs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dcojmran.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sntyyxkg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2muibnqgb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pwavtwuy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cxtnfivx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pmqivcci.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zjiqbumn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nklpmugc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dnxeqcew.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mcoxhhrj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2amvjztly.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohbubsxg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eytibwyh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vsusaolm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mzqqujhf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mhxfgqkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kgjpgpvy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wgimqatj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tspsedtf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ueavrcxx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jbpohtiw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhhjxfc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hyrtlvyn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oietxwbn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2macbfezw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sxgsivxy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lfvtnaqj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lbdtbwdo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ysjfduxg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yqxpqktz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkokpqrx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mfjtszie.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hgvneefs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hqwkjisq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qzkefhot.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lrhdrdjn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2aswgmrrg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2snqxlasx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dnbzznia.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptqlzwjp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ftwgzvwn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cmoslumk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2eaxgxovt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yiyevexv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yzbqqoud.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qhfafgur.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2phoxljep.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2imwxtnew.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vhkypsyu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oxgaoiym.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2odwushsm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2idoyyaux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isjqhgsx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rqmomerj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2crffoouf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lavwxath.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tdhtwsud.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pllfajbp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ydjczpfc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2klfhrjqz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ypicegkf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bzwgmthg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhpiscxz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qjddmqrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxdgxmfe.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vdurczvj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tyategtu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jhzbcohp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xbwyxyss.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wuojprlu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ognwjrhn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sihxekcb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyteruan.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymnzipvg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dtgbzrzj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wxrncslj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2npqedgop.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eorgtvmq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whxyctwc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2apxthfdc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywriluwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwoissk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iracrhqd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mmhddbtc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2eutqbikr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2riumcdkg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pqywzzar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tnikthxs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ssqzjkzx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpjogll.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2usmpatgu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2toiyjgva.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gxkmsvvd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ktbbfjlo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qnepcvgj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ceoqdysb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wbxytsed.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nkigfvwd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2peicjndo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lixvqtsi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bftkqkfb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oupdvwst.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ljrszxka.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blruipyr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwcdyfcl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjdfztyk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2chxvxytt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsyvvem.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rphxffsv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clwuwupg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rsqngjpo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sicnmqyw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ypomdjxd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpcmmno.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsvksxlt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2muuxyfrs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syspnqda.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxwbuqcz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hjleajhy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wwcrcdzn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2syejcxqh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2aueykqbw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tvuudpqc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yzipjzlc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mrojsjpe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ysdwesta.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dsspxhzv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gprccivn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iwxbmjop.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqlzkbd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zlzvqgwe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ffvyzmxo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wsyffdgm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ruvkdzip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2adxdnrgp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hqazribc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fuunqxkq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ceguqyuc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjccwlur.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivjryyqg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ianhbath.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nipertym.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2akxosfcw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rgyxncmt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arcmdlna.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2eixvsvco.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ikccntjl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mybpbloy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qoskcqlh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhtvzmce.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qipiemxg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rjklpwww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdsmwhdt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bybpvvxz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwhsvutv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qkyymxby.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmacudhi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccttfdrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygrdmqna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqtylrsv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2arsqxkox.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2irpcxtrl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azibbahm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkweahq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cjjeaqdc.html


<!-- 参考信息 -->