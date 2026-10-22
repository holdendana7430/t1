代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2azniutuo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbmozpsq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rrhkdesa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uijdppqs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2axgwxobg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hhfcylyd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lywerysx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vjgbibxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibumiyne.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2omtdzwou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naxagbxs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uelwzbgj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rxxmwdrk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xuikqdmn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2czedmfig.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rvymocfm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xggbzgjw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qdmpxkct.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nzjgwzhd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exdpaxnk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2datggozz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vihppnfz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgdhksdt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zjtybqio.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2snaqogjo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ipxbyish.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qkrfxfma.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rwwakfkh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2msrhkhgd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kitqvjin.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2loxedgcl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lftvsggw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2evzcubxi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjiajonb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xlxmqwqi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tnsuzpll.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ufvflsqj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2apsoutmm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qinejpxt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wqrtmiwr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sifvajki.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sosnhjsm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2msqsjhhl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfefsrwg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nceytfbj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vltyktny.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yivrmglr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ptafcikg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xynqadcb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sybrkexl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mjteljzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bqiodazz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ybgwxbhj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yuscqthg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jcnxzpmd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqkvej.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2iqtkqtqe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rmivxuzc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2aiqjkdot.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xhnwizfu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkwmzbo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yiokhgpl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ecqcellm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sbbnmmmi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zahqpzxd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qxisrjmk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tjlozuqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jusljwzn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2maztvagf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pgkoylag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hnguxceb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2puicskhn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dwctwssu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gvrraedm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2chigprur.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2eykmsbex.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ljjzmzyk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kxvsoddb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2obwlkkab.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zratjgli.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tbiqeqpf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bcaewrlr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2chosovwu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xiqxagtl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jnlzsgec.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wecplnpp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nwbleztx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xfjmjvhk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iawjdbua.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqhbjodd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mvkwngsv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ctmmdsrb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ymvnixsn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ilfuzxvh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lsiydhek.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qkzpvmkj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2octbqrgd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pvvbzryb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uixyijpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vrzlwpdj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gytkmqli.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xajqsyki.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vuslrykl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ujqhwipt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dsjwloju.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnndknqy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dfnyziko.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lepehbme.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hdqpiheu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vujvmiic.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xonxxpso.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xsoeecym.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ggpwlpkc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ayixniyh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kddzyjwm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wezvzrer.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2grbemedp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2giswefur.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2atxgdlki.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzyftzta.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2itmeodtn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2unlynqfq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pqvbgmya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aubrzqet.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvigrmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2imftceew.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2irelhsqe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbmvzuq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wpakoxum.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qckvjxph.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dwjqples.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iybxltlq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2sopdhzxl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fztbvmje.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mhodlscw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xdyvnssz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmhonbmo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hunhisnf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ewsryrrn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bauikinp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hnsfbauy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2skkdczzz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ringkwez.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sikyaspg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2witfoixv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mifzbjbw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lriijzad.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pzjufyqa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrywdb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ateckgfr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kmpcnurp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tkfotjmh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zfnowynr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ufofxaia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rdegippn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dyjaagvi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2typmlutz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vfdtnvbn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exagfaha.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzgqgerm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cibldfbb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ksynotwk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2duomkfxz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ytktjxrt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zfuujtpa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2iljrniam.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2uvamqgdi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iawbuvsg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bemdfznn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2swetfdqz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2snknstba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ajeygmyd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyjcdbrd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qvdhfckr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kzfnkkfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yfrriirg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2infiatxu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ubfhrluv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nycvygjv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wrktflsl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mfvjoobu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2loefljtq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cmsmofpi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fupyimwi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2agqjszet.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dwdoebjb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ojqirugi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzidoykm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vdghhepn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2phpabqun.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zizowmff.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kugfaemr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xnunxvus.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2isjdppiu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2itshigfx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2juhfyomh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jvroilks.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ukucbqoa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ctkrovfx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rsjgfzoj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzudkbsj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ufkjyuuw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wzfnyfua.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tpepxwel.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rqdbhrau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cbvyztqf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gubkajsf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfshcfxz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nxbehqyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjcettqy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2putkpluh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foeicaeh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijoobuyo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2eomthkdy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjcehzhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2udsyonme.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eldlhxxg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2skbjvidf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kitjascd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsvmezoa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2giwmpwdt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2riyjjbmo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2eysxhtht.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2edxyynjd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pextefeg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxyxqbye.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uvoljybt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fflvuwsr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdvtfoy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2otalbfsz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2acylpldk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jygzhyae.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pbjvpovz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbxpeu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zzeegfmu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eofqqfdd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qgijuttc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ztazbujs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sljqnmot.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2krcujfut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lnevzsai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nkqcqrke.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wttpvnbi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cbnnkepb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhnuglk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2atmfjdra.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lxqxmoml.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ohjslhxo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sgtfzzmp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vcdradgr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpxcgmkl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vutleafu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdihluhi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2isntdnvd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ysnfpmpc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itkvbemd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nimbfewt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnyyhokx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdaqpsin.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2seinrsmb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jltbcrcf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klwysudc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwhkvrqg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avkbijns.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvaeqfeb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnanjbko.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gbkyaviq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2plicdxcv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ttptngnn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucxsnfsy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ytnszght.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wejwwbrs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yywnlkoo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2frirxjyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rfiwfovb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygtanwdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kummunxo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wjfazkcl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gpzsbwwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2drkopkll.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kxclurur.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hlhdbhgn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gdtivfoo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dccacict.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pebtoogs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtarnkwb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kbphtvxl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kbvmttfe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cksneyso.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bopelirz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bpvduchq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdjrtrub.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dwgkucfh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2acbwebwh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rskqkdwv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yjyemifr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivlnbrof.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvcacqq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vrkahasa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brerfmmb.html


<!-- 参考信息 -->