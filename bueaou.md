代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuzpmnpv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2txhuhhdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzdgnmor.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vmceotsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2liutczes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vjzvndrx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jeuoegvj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2auiirzbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zchngaip.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ckaamncb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vpxtxfkq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tdbitury.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irgwasyj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rkxneenk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tblpxldp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rbqzywgf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgpffln.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qpioyacr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhfndzxa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nzeevovm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dvlsthqv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ocywyqhs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jicocugv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2onrvadhs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zkvhyeya.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fbsoitpx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2towevbnt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qkewyeme.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hwokzjqq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ytrvcsxi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yllnssjg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ukjjtgqu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hqnvhhrj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sipnlglc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bogfkyxe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2udkmysjk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fesffqjl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hhxowdly.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2owthffvd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xjaogzxn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2otzetilg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zjmulpfo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ipydufoo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vjktfkjd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmnuimfy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2affzpywt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pabnaooh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hfvpyelg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlpyrudq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykznmzto.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wuwzpdjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iuirfker.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwqwdbeo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kcmvqxwo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kscvaedl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cguwrlgy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vbdcgajx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ozqkctlj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2oxgixcuh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wayrfaoo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2doiptstp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ifwxjfwa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cmnmbpth.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2defwvxtf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2owdsbkzy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2axqzeuzu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2sxiwflnv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fgnliuks.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2llsvcaae.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jxjuicfm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kzcxleio.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tknevvjy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mhexczpv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jmtyyzcs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nxrwjqoh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ajqkjsby.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2liuhlfnn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mbedobyr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wdhketju.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2itskzcvp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cljgybwb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtchjn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yteegemm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iwbzmvya.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xjcmetbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yzuuijxi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gzixwgtv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wlwhxwkc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qegrchgb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mimtprcx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wazgdtxp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bbqsyjnw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmgnki.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dlkqgpgt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mdojkwwz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mrrdkfrc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mibylulr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bjgbpihq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cnbdfwum.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wjygvbnk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qzabagaa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pxctkhsl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zpmpblsx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qgmcswew.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2evyzvyuj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjtmgbii.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qwjjwfcy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2refuxvvh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2evjgzvgm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ifqpffkd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wkbdkpzi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dtqzlsyb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtgxqbp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbynleb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bvvytply.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pyymjovj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sndsisrb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zulbdtoy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmuzysd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vabjlxgh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ngjfuswk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fbstrvkl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sttzywti.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2aeztkgdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yzbcjnev.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eiojntnm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2opkaqjxs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gbcbbjwx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aljamkzy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rsbhiegh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iccjehwo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kddmdjij.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqmqgxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhbomr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kxggsfvm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wekrohpm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vhialvph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ovogvmra.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2grmeojna.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gxjopzzl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mbbmvezj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2irimorns.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bizhvjdd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wygnvqvm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2elmnckal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2njicazfe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqtfaqce.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2denzkezq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmecdbt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ndtqdauw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fjwsdqhe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qckowmvp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wcrmawlj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rkkpjyrr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vhgrlelo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bwjeiuxr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvvgavrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tntqasgi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2myhehhiy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mxavxfax.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ufppuiid.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2htflpcbl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nykdxxmp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fwlinujo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xwffguxj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xrwgjwus.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hiocbdyl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rrgxcyug.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sjytbxzm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dkmeanta.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fxiozcoz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tqnqzerl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ryaccvak.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dottarde.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfqewi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qapcwlhl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zhsnybrw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdsyduro.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysziykem.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntaiqoko.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsdyhmrw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mqcoaifb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnkdmo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ssyggrfh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2adqnqilk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmsuwjet.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dfgjtebf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oxvbctde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ioirjagv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sthawtak.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2niaoybgn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lchwliji.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpmieoag.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lzewxakm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nniomepg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhnbgebx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gqdgwmzg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wpkneqqc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2grzmbprs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ezaflrtv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lxlusmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qojxyzvs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bznydjmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyipdwfa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyevolph.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cmfrhfhg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebvxwiou.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bsersmue.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2snqcznsi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwfznide.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mgxeaaqw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azwwhehu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qjqvvszm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgqlumwa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pfzmcfgz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2njvxuvyu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2msqjmmto.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dwzccwcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lerpvdhk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gaukzonc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gezqsgqc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxugdan.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cvdozhkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2sakxxeub.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ovrdilce.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xvisriar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yossbdwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2idnsqjgo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gbheurea.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pkqvqfeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rmdzvtpe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrimrhwu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnxetcdz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2uvenncfu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hlefhtlo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cgrlgxyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jswejyuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rwacuxgx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dwdmejsn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ntloudww.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hhnjgzyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2inzcqhva.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwhwtqlz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgnultbe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avbpoudl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tzvsmpdi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzpbeqk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znzughgo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpaokmf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjighkiq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oieodxfe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zupxkugq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqurgjzx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifgrofai.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2voniwpdl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezqexmkd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlgffwxt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ynimqiry.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nrkvqfyn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yvkyjtsc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xgznsqwm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zoohrbew.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2okiphcqa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fahxqkkb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sizmhqoj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gwjfjtss.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fckonecs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iwyzymap.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qiexdryf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nmvgijum.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvieiokh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwkenqoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kqpmzoco.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zfjkfijh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2thatvpnt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2unofzdgd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2memdnapi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihezmzfm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egpkmtvy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gjtwqcvy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wpppubyz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2orwpntqi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tnnsxulv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojulxzno.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2glicdmtn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2alvzcaou.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjqwoawq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhzirgve.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmcxpmom.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gslmceul.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2advlqpys.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzhretll.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpsicsjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oviqrkgl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dscemryy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnczwjri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zypzomhh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlytmlgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjtxbzux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sjkwpqvr.html


<!-- 参考信息 -->