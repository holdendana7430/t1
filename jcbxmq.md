代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ieefkybw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtwtcrs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uchktbat.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xbrsvoee.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ytvdgjjk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojciytjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvuzyrf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cqyuazvc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xtaowpqi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sftbvnbt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ajgvszql.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tdaoirkw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qnafxkmr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dwnhgqhd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jtpiiqcm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zbhnelhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvdbnndb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2erjnljgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhmjexxj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ucfbkopf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bsybtwgk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qlgltmvs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jhpnlwdk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uahtfiug.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwamcujx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qjhsmzle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xbvjahzj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2niltnlju.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vkdkeymx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ffhffavw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjhstorq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2byaccqgc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wgpnifwr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hgbmrzso.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2goseqjer.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vysgzlrh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rzypugil.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kxjfhfyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2njoxwodp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wwdpbyhw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxdowlbb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uwunjiem.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cdngndqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kinkjvxu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qiuaxogp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvlvogd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hbmrjvzz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sicgvdfw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2grzmsurn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wptpcrfw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qnkukpix.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jnpwostw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2egdmlmkk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cckhighj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lhilsqmq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vyvkwnxo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qcylmuts.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zwawotow.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2irxqrlog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pqvmwzlw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqrgcph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ytsyspgt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lqohzmmz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nrazzmxo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bzswggwj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jnaxudyz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xvkkqubc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udvocxhr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rturfrgy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2apwvxvum.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbsdvvcq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lzvbqsjq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ayfcnwhc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wfqjxiab.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gjgdltyu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wxppczud.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zpddqiyv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ehfezaom.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2daefvquc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pblefhah.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2oihpfbkf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yfbgjvuc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jtpbxmqk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkgoalpw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vcowafxf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2blibxygn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yforyvhw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fkavqzou.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yozcwwny.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jkkfapea.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2llorqelf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2iorheiub.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xwqhcmjb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ikwwzwtv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2piazdlfe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uxxwyaba.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dcefbbnh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2souixmyx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2loqsoksw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nwqegcor.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kgeyrgxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wbpfnlio.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zagmeman.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bgcfqkcn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzdaats.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jbhqeruv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yraeskzy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gsedsaez.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jmwnxyrm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aaonwizz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jecfyzwf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2utfjlkip.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ioarvdwp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwxkqvya.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zyrrkqmz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rfzityhx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tkxpvqtd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2evrhequi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xfyxsrrk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2irxalsiw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2erhreyfn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2husbhjkk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pyjxtimr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hckeegwl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xyggzwbg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wzvyvvqb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qpplinul.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sjbspels.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jemmfokl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2oujusyzg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeqznnbe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wbcjdnxw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bdlqfbxi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2esxraccj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vwplblto.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2frnrfyfj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xcbnizud.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bbyezmhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zkzjfqtl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qtilxzdl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xgskrnmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2efmnnlmh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zkzvupar.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ijkyzpmm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqyqehq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nexsvkmf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkewbiyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gjnijqaf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jnleczym.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fvmjmntm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2skakzxwg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kduizjzm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iiaqicox.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tokpugut.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rsgygckv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvzilncu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2laztwcjr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vwszxdls.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2floapqvp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2laqtmqgm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fjxqrlsl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tsxyvdmm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lnmczxxs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2baabkhmk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2duyljcmg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vicsfmid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcclqde.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2npgmymqe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hqytxcdt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2imbnewto.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rqohircw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uhamenoh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ffzsigwb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zxiuqaxm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2juptlgsk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ucwiculs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gybfbnwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gpnrvctz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hdekahdj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvpjzgmx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwiihjmk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yonpatya.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2sjbzdlce.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqziwg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2munctsht.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtnmpsi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pgbonvyi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eifgjyts.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nbsxrnwi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2otzwimup.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jcmfuucq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fadgefev.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vdltiiyx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxdueqqu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lijjjpyq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rivcdrht.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jztqqcjx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2azaultar.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfrlwtxi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2msdvomcs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zvkfvdqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xdnevnmx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rhbclfrf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2optjucdv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rlxtnzrj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bzxrtmbx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yrtgsvzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ofuxdahw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2iqsacvgo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ycjyfnzs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bxoarhwb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2huqxdbqx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hfbbpfpt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wirrjtfe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bfykropx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zeawdkqo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ipjgauut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oobtpreo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zcuacehc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdprondz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pdszdget.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lkstxqla.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zuxpupoo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2swaagkhr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hleznyic.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwrqfjsi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wrllzxsk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccxftmoz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tnghiyyy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvayazfq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mrrznior.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wuawtqfq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqxlreci.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pzhgrqqf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zqufkjaj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnnxboj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2aoacdrdn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaexkulg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tmaeebrc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yqrykrvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sabicrhk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kerbxvpl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2twkwdjie.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mimkwqrs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rmvwprra.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2itjrjcwx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jexbfiql.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lypsvebn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dpldfzsg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2twhzksbv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iccpzoqw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zohgdfyv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvnhknv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dqaluwak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2beevmbjj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dummfhuw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2scnliaam.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hjbbpwxr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eabigcuz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2momiabwa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvjggfbr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wexsyizd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2holjjofl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcxnfohs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbffequu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbjxvwaa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqgqoxpr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eplyyzsz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atgtccws.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olvqnyzj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nywulmnm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lodlyvko.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slxpmgyl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ueyvkzpe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vykfzmmd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fjgwueez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xdakuxlw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qvjkrbcl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2difwilpf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkmjsvyg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mgwrxiav.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dcbprggk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bkcfshxk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jujauevv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hvuzvfjf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sdzmtibj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vlrncljq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lzxopsaz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ishkytih.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fkkvxxpm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mibztdsx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jyhspvaz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hmnbebtg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snsajacr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2arweuvia.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2khnmbday.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xgaenkmu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sajyengj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ynaylyml.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxmwhpmm.html


<!-- 参考信息 -->