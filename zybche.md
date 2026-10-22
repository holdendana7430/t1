代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlnsntsf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tddhfxrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prkukyge.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cepmtpwv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zldgrbje.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wtmcspdw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vuvdkqro.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kenbltye.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rvxudmns.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vszfkyrp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2souuqfdb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xnsukuif.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bdpskrhs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lufqecfs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jzasnyot.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yixfpmfl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdidmpsq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rwjzcaen.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfcxbzo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ndliwkjy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ozgvwell.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vtkkhcgh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gmzsdirc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dylnqhhl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2abfitdha.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzxmzis.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wpfpbtkw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yyptuzvv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kekgbcji.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ucfhvedl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oxmgxbkg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ssdgcyef.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wqjjgvce.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqdfstt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2samfnhfp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2awhmnlrr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dsmhpiyq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpenpwfb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2amayrkbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cxpbonyr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bbxkfejc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vaijlqeb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2goskstke.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ehkypsud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2joycjtsk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ftyeosfs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zolbrcuu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jvgaxiaw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2oihpjejn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tonvnmxn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2oopprbrx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jvotgxpx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2omvhuzto.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2negujtel.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdznzhem.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dyitksyy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2drtllwmn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2awwpljsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mpoeqgtg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mjkdtuwl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2claoxfol.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fjzqcufp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mhkeolio.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjdzsstg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2alhzjzoq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jptrslbb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kwfirsfp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tmapfxma.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dtfwpczn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2glwmikei.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ksbfsqmt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtnogcu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2iaibwkfo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mfejfydx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kybxrzma.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wvdqofgh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2betjmxqq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hjaxeuje.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2enqsexja.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ogzposfh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2caegjywu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tbqsbgic.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tszqssbr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kcnyadah.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dkxbetdq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lctopmdz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gyhnbdet.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xjedmnfc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dkydbral.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nojaulbh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jckhneps.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kyfhtwaj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ctwkzwms.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yylcclch.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ryjurqml.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vcaphcxz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sllbvbni.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xarelthw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bnidnydz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kqqtgggp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oglvrvnq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xvxwyqav.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rsoimgmt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mnjdhgtr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ierblutz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dsgmxwqq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2djbwaary.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2oloahjif.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ropnprxi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2alzhjdyo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2urheucqj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afvqsdeg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fazdzwsp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xmuqimww.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzyhrut.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bqmyczgf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vyglmqyy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2tywvsjwg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yzapkbvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2reiiuykw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dvcqfnjr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dkqvfzac.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gcuczrff.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2epdsxogb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvfquar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vodsbaex.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2smscngvu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2akldbzar.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhjurhg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cdagrjhq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqfwyop.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtbdsfpp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgefioe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yojkgfqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jmgvkjrl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vhggmord.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ovkokvwe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsezwdyq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bwhzlgqu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gntvxlqf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bxrvvhrm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2azxxboux.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cchzxlez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xfzekeuw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nqxycpff.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mbcwjlok.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fhdnhinl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dlovzsgf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2exaqkryh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2moegdehc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpoofj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2juhekttr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nzilvaeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iswmxzpp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ikkifwrx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qxpztxpu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hbaywxxo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vjlppqry.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zraehstf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hcmivgmu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nwehclne.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtlhdezx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qaazuenj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2aqqweefw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2afmxxixf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tmoqczsk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bdaphllz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2acryfjuu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fubkaykh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uwghnnpr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spkuucio.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hknrbdwa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hzuquetd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uotxkvwh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wviomojt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mkaqigjt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rkluhdyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2patuimfe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vceoifbn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gvicxwxo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sxesrztd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bjpnbxkr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nawwrgwi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2imeangey.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jxyighwx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qwzbsfzy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zgghmdqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jsmrgcgv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mbuiljyb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pbkfspae.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gsgsaeyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cneqivvz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zxqhztwr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxnawjs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iwqfeicz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfqkmoog.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bjcqnxyi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eicbsubg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dklzaxxe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2euvcrpgb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gejygvoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcmonejh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2musexczo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvstbsnj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ykpbsqlk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dbekywrv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmflarwr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lzcuorov.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sjgcuobn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zrwobztv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mlayayeo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpukhsyh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlufmfha.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvzwodjh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2aaubpoxw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2skgmvyaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2occsofun.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncblerwa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zuiqoous.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2czltbrsk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tolfcamc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qqrdpdkh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kxzmilpj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icudwadz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aosxjcfn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wzmihvpp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wewpkvsp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yamerwux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2shrklieh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ettmoczl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2abhuwdji.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkwdjqyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bepbsdpt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tjcqqifc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2etdyvmos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2drlsnfkk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lrqdnpff.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kjggnego.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kidlgsox.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2etvaghjd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hqhwskcn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tuqgbepe.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2basaghnr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etcfszrj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scyiiker.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqzhcnbu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ejbofzhm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmtnksqj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntbflcec.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gyhmgdqu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wymroygw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwazadlc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufydxsiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diyofcev.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxdmiqwk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqrrjfhv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbkscbcy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahdejzby.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jqwimbmr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dhzqqafy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2obwoundr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hmmiecej.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xydehmmx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qilwuedg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2obcbotgb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rxexxvph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2srtjsobi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2puqqdiha.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rcwjlmrj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2znsujnss.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cqnqwpir.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kjofilpp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2idbutgvr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zmyghtyj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2owsgrqaj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2apljgjhn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ncyybbca.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeilitqo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxnbroqx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hsotdaqp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fjcaafmf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sziwoynp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vfmtyvin.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffakoaml.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ubxdnvus.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tfbmxyin.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noliuuyg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zntcutgx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvlchdsy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stomsher.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mejegvcp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sspnreto.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhfikwtj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drdtszkt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayzsysko.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2clguebgk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2isaikleq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wndgctqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfmprila.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fyttpuzh.html


<!-- 参考信息 -->