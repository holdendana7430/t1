代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ogvlblyx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfjvzboj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrblwrcv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2suuwgznh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dtkcazaa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2houjegta.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kwpwdoxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vhdigiya.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvkjqhdp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bkgoxfox.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hmhrxtes.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2whhxkrjh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2akweqyxe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qilpddcu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnoqtcmr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kkpcvipg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vdwjezup.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xdexhkgo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kcdpypff.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fjugujww.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2khczdhjp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lwrgnznf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvrbqhk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vxcxhghh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gkahpixz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfwichm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mmcdvqmh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2neqerxtm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ktccxgxx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ygzobgjk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qyiwugay.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gmctuhps.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gwiinkzh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aherowdg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fluqmicr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vljyqceb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pbbjzygb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dltzyobk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wgoudony.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2saovcqza.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2smjczpcd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2makujfjb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyonrvun.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zrtxnxrc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lauamvht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsusbidp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbskgxn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfjlekwd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjnixiih.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjzkkbdu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yccayksm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rponlbmz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qokjvfuh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ncjsoyxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2drcmbaaz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uxocuojs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2akgsgpwh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jzxbeuzp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ozwrpfmu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2floiwwre.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ugdmggzq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gqinbrqm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xmomkkvu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eabpxcrw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lhthvzhp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqvbbhn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bleuaevi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrtgqhxh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rqowenzk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ftxqlxky.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uubjjoda.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rvtymtet.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsdqldn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dxrgeztg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2idepguww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2minoaabg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2achoqtxy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2acaxbmno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jygtljxr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmjxbwbd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bfvddxuv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zxqwnjsj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2haixyind.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hgqoepcl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ailuyoae.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jepmnvnv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ypdcjars.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uyodvulf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xkjqngum.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suifayfq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sckxzcir.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lfyastoz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ddvzryob.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wkxxnvig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tydtuuiu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jzzuruyt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hfigbrtr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rdnzjnfo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gczpcama.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2atccrjfc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2auckqvsu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dmpoyfjg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kdwicqrm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cblfivkn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jolodjmq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlqujnl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2saluhzzc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ogjrtnpc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vprsmewt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmovjqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2elnuftld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yidfgbjq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdaztfod.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2bymwhvrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbxbdrp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zepazpki.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wyrsgkfq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nxddykvs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kbvocldf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cvabnvmq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntsbyfav.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2arfvtokz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ehuttxdz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmkcizs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ujvinuix.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dmilxbnw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcozfrzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdmwwfuy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2arxwujmx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2myskvvkq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qvhmtvpg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drpggsbn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2frauaomf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ygdehhqs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ntqsgnas.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2inllhuzs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ljctmvpp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ellilgps.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tpkhlzkr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xnixegix.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xixvkvne.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nnefakyb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uikuntex.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2duojmyna.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nymibqmo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jlcgdifv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dcdqszdf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fuyohtby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2begtsqqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zutmhjfh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dojxzpmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kcbfixfj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2stqtznwb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xukegebq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vprwnocu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvkqogq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hzinwqrm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2adtpwlqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2evktnzsr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2msppsdje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrcrigpy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lpqtkhjf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jnnckffj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yvmywztw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dtazckcb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qugcujgt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcchhiku.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2efzjgton.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hewcwdsc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tjnnnzpy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jtuagdkv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fpcxwfkk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uxbhqkvp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fcyhdfbx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpgprlki.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dwfqdbad.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwzgqmfi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jipeqxnr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kaemmevs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gmxfzbxp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lvtcoyan.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eysfkcak.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ejdrsvml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2snvxiipd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qxrzfapp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fhdahpmz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xztwvksl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qecdilqk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ethobgat.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bcgixmzr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vkooibjl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uskgnzpj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2okbbdxmv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kcjysltg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tnlziunx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eicofbkc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qommcgkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftlzhedu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hdexluvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygkejtdx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2klbbslrm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jwqrguju.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mijsvmin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dsxeurdl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2owgqrqtb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2onbjioge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dxnytpdn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czydlxkm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ncswxkim.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tettanri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uetonrfc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfawspbr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hqpvcdaz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqncudht.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjmxumd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2suflhvgy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vpztqwgr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rrctqcxg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uhgaigur.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wvacinel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2meelckug.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2btoqkaig.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rbqikbpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qiaxwbsp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2twcgnfiy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zoztjbww.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2odzvwtmv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rwpyetgv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2waeckhia.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wttkafdw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwhniqu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jeeobfbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tpvsdckw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qikpgjue.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nexqbfco.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jqpdakvc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gjvlvfon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ucjesjqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qpvnsnwm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmodubph.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhuprpgg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kbgijkre.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pfjgnhtr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnvflkii.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxeaurir.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwunpiuk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzsxeb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhswetlk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udnqqeem.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apckrefl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jshhxyfd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oinposgg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybdrxprm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qctidwzd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qhsjeinn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwwvizs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bnutypgx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aeazrrrn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2erodjsjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gevielxc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mleylwoj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2utedvyfg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yfarwjlo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhtkizox.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zsofnboc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsklflf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bqrkepap.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yhiuicdy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kttkmqhh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2svjrktma.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmwouvzq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tavykqqk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ziokpqia.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjrtvqac.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wicadypj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vunhbtdz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ypfmfkof.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2grtroriz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tklvgpue.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjjxwzps.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ltbszyue.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hjqxcuqi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axzwdkpl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tsmjmlbb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gitqqsaq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkfrpwgn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qqcfslrp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aoaqtdhs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txtknpok.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ribyhsma.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcjmbfjm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypmytprt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dyukhjuo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxocbhyi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypzzbrqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lfgfuszf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rwfappwd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cldcvpgl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hjaegnle.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ztikcmwr.html


<!-- 参考信息 -->