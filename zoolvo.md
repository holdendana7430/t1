代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoyemjkg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mrkjgljf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rkguedif.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vjfctejy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kszwjkag.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rcvxfgoq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ybktinkn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtkrcwd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkzybkt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nvzueldq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jnjhqzgm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iwppajpw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2idlvvuuc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wgtttnfe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dvxrbfhk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dtbgmxpv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nhzknxkv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pzafcjtz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zapsqogi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ppzrkexx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ryduxdkc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2esyqvnzx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oktsteog.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eyrruimy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jrkgvffk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gejidhok.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jyuylryt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zlsaplkf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dazmfncu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eezgnuls.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ckhpaisl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lamhkmdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ojwpafey.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ofwtnomr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pydmwbaa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iqzxacxf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2enmgqmhs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wwmemtlt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fhmnylfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2phwngiqx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gowzvwpt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyrbzyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuogwfpe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qerzexia.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dzewxati.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhxygnfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cretnswr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqjmstsi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cozizolz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ajvswjoa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hftwflfu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hagsnpdb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gpltezjv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vpufpuwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lfzvhwon.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2aptasphj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tpviaxin.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2teakoopt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2aeebgsul.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zutlaxfr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fzypmnjp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qvgolqzy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zacezzww.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2irfwsxoq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kaozgjog.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mzqjiwya.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2glrqoeso.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sdehvtse.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zmvuwanc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uecwwruv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2myjtamyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rnjhcavc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lijjcmjy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2scbcgbzk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ouzlioyf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2txlmiejg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2snlalwbu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2drnmybif.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ijlhsusd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jkvcczxy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmirhsyo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iypbalip.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2irpjqjky.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sypfnzrl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wjzvuoam.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2epyzfatr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nfgkpvzh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yxmvaklv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xqqgmowm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htjdhywo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qnlpfdsb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vgcpfnzh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rpytafze.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rhcdegtr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qasjgjnw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xkrpsmak.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lpiykjds.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fmcccmqz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hvcozoea.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zeaufmey.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dszajrey.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zwsanpbp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kmtakfvg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdjfqacz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qcgcvyii.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2toxuuyhw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xywzgvgm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sprylqib.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzeyugdq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iglbkhet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2smnimylj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2obelaajy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2apkifgis.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2inkcwrxp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcekcddw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ghpfmyfk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtnywos.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2khzldeyf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hifxgfvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kopcrkgm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lykqhqkm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pdehwatt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fafdhwii.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oryaqoyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2byhzsaio.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fgipafmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2foxwnvep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tyhucpvr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dresbafv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cogjazsw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2djftbiag.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jemjnnuv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dtxumint.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gikighma.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ucjoiqlm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2imzipmzx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ttcskmfk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hukfhsic.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2njnkilth.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mifayidh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dhuswkmo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttdnyoxl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2otzlnleb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kviqcctq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tohsropu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tpdqqqqq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dmnnffwu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2unhhqody.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ichdzznp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqyhxgo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ylugrkdq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lirjqqlj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2msadnsbi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbcpxiu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jmddtstt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gmowdhsg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lybcfwig.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oznxresi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ilcmhbyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wsxcmxbd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrenreh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kswhzvxy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lauaqups.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bxfiayim.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rvxcwmvw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sxjfvlqu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hnnkituk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uzljygki.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xxtyfbbs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbtugmzw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yeyyspvv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2palwrrdi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fpmtvgmb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bcbtjblw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vocjlvio.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ekvjrakh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vfhaholp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lxuacdqj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nxluivem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmappbzo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwoztdqw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bmjmlsrq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mmmuibeh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cfgabhxm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qtkmgfrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amjwjqkq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2awuhcjuk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ooggzicm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mkzipxoc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ktmmqnil.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kgzazgxf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jlftuvyz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cecthckq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxebffwn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hjqwtsao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjyjmuyt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pjgpvnxx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tkbyhusu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqauhiox.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2obpljoyd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yqtiqijn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2twuzzmuf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uaxtvrbd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjlrao.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2thjarpgu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdylqdhu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dfdakkye.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwzihtnl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pcfrnkgq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqcgmx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ddaducyf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tevpxqps.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tfszqdxb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkzinemg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2oqbizlwo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pxaxhsio.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yfucwxlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nvoorlsv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ddeyuqbp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfrifnt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lswsvqaq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wiwajyje.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sztqljnk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dcszepwd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jcfhsugg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jszfugcr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2umgezsji.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qbnncnhv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ctuvozsm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ornpbyhc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qbybgbiw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sjbwavbk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rciyjuwq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tqkxgvdw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fawdfzfz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccdgrjld.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdbqibgz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pdsohvcc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ywkgklme.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbvzvahe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xeyopcuq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfkowwwz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guorouii.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2svxpvbsv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubhfrxyu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmfaqydt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nadihrud.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkfrmeek.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzacvdmm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gufbyznh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rvzrjttn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mgbbjhvu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2coizbapv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jybkjkod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hmougtye.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fxfdpzwo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2agwsxxvx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2azbzyxwm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mcixsudk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2impijxfp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rgffsxro.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtfrjryl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ireabvyt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sovlkhjo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dvbggcft.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2opqbrupa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjaezcv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rlmtfpqe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zmkkcbmj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sstezyrs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wkatxygg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ecfzhyny.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nvgepmgq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mdvddytl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ftmoonwz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxwxcnym.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mvwugvcw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nqdienbd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfjomyme.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjfuqn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftlmwatp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fazyqhvr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dvzskcsb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wilivptl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rolwqayb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjtjxiii.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2waukcwit.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nenzfpju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxllwu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwktrikn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpzaensn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zutryhlw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2khzquekq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdikjaec.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mhcvaliw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ieyceebs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ssapeivb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xrgopnbi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2arjlrsaf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wfvnjfij.html


<!-- 参考信息 -->