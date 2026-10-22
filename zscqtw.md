代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vcjxsluh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikxsaesb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdovcgh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2giesjqxd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yuypamko.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pogrsmrk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2arhorwkh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zysfjezo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqucwhdl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hlxgrwsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aldvcfjc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pwrdicoi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rdgfauub.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tlkedeec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kbdvebad.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uyihtvqp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cuwjrmtw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qdeajaxm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kuwkadfk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mbvltoqj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wvsvhuxj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2onocculb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2upmxptwg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ckuzmmmk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2upbgeyey.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tearccht.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmndgfs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zzctbbhp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hyiimbza.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oaszllxr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2roeleiab.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ttewtgmf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2grxebfsy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nkkldjzk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ohodmiyz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wmkkvwzt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2aibvehub.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dsypqlnx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mjwkqeoa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ivxiokqt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tbkkqfiv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfouxmc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xgbkfbvs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvrbyta.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nsicxxzx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xpfycikz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yfnyzxjc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xikdaemw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2aqxadovj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vdqaujxw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtgvjfo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qonyorwr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2istqafdk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2iiluujvb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uwdlgyaj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cumepnqj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ydxmiihk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dblbupdb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jsszcpmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ovodmrtv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ocqktbzd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hvksfldy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewocnegb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2feifdigp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gditktuf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2htkxiqnb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hqhdifes.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrognov.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jciffepj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxcnxju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwzhtjf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkdsrco.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wcvtnsbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ycskhwga.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bgkrjxgu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2acfaxdii.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2drpucxql.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2navtujfv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lbbkrbpd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2epsztmvx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jvadlcos.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yoxhqpvd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzkcjwn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wipvsxch.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aueotgso.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhhscxsp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gmnidudi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qinsftxi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mnulgqip.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jwfppelo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjkztcuj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qazggmhi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lmagdiwq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hjvcjftr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dncugewi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yyagzust.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjcpmmgs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqzlwag.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hagxckwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ujbopphw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fverfelf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxcmbysg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2puhtfztr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xqscnzmx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jwsxgmga.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2idxcdfcj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wdygkbrf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ucxgqhxa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gsbkfhbp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wqtqryqb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yabzcsai.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aylasipv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hpxipimq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjgvojjw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pbdruwef.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2eugiafbv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pphulhhx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oiiuoydj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2piqizwgh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pktwgjfj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfucdck.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2awxoezml.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tgklqycl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2asvvmatp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iedwpvvc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ilvbmfhi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2exomykgz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oasmwmym.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ldubgwpo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mjyvavwv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jsxrddch.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jctqlkde.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2roxqzlet.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dolenwsg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wxmicrfo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qcixmvyz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kczmleeb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fyvjsght.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgutmez.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ifnnmdoa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ydtxatvz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wuzqxeaq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2caxrhaqt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtyuehuj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hejolvso.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uoqlgeer.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ehochsxq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jwalhhwj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gfwpnoah.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qmlseubf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwlocu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bwspjanl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jvxkclfg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lwqludaw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qfnriqim.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gmdacfss.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wbznopdy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lkgzxjmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nahtcwlc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pzeiwkhm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rrrmqgpe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zvahxgbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ekbanwpc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mfhtqife.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nckqadsd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nycwhyif.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mtzblpnu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gmmmdass.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqcjngcz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljetjart.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jymgchfk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hpplmffg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zfwvtfxi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lgmuafwc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tjoyuvxj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wckyfmzu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nawgyigm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2klhkjntk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjdbsbcy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jezpzbqq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cucjyjog.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mzhtpyqx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sclkqwla.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fucgaogj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ovhyphqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vlhkqaoh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rwcycony.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edpvmbou.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2immlmvin.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jdozvmej.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2guugesrg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mehhacws.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vigglslp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gpbiovwa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dinrssuc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sjdkhvvk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ugslcwvl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2towytkof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zqrapblh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dersxttm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sqvgdvke.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gihskxmz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oklwqwqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zyqvqvis.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ghpgzakz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2slvqmpev.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rwiagwmt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cjbhygbj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hxasiaof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqtpdbwv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2axjnxhse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltbfztqm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggvpwkaw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2smmhrhcq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnabnxzt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wezcvbkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2grxvdioy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmchcljk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vwzknvrf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bikdzlgk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktgoeimy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jllkcilu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zeclgvrp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqszyci.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xlhdiuku.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vfeiobug.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2auhtzwkv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmxbsbm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2odmfuzra.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qsrpbugv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ngubvdst.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vefzzntv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xczxpfxh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uyuvpuwj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2segqcmdx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2umpjabls.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pakgrbof.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fdcxppxv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kfxypfkk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2imnxonwx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hcxsxzlp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wtppkbey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hkgalsul.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2souymuvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2chgqdbfj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hacubsar.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2blzzmjfn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rgskqdhw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uglskmfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2awhhqequ.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fygamchy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnqcypyn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ivkyxtre.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qauwzrbe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bmoqzsgc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xydqlcua.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oayinjbh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mebzgjcb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2appmvbrv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qqrijlbm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxxjayds.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xubctlfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ewpvxldl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uldlgzsm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwbhhjcn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzafktwe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jgifznus.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pcjuxvcf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xsgzwjvo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yxstissi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pvflmveg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxihbanq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwpbswd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2puwurwez.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ayjfhpal.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2odddndad.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2clvjtrdn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvkjsaqs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2utkkhakf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iyifvwbb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2znpgeosg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jngmtlbo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2samlyzqk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2opcmwset.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dphlbdtw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgqcypfy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqzjjqhz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nxleeuyv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lbukkejm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2awnvxlmu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gqmubxkr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urussxsx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2plqlmasn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2phvdiixx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2laczhcwg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szysbgpk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwlzjah.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlfbjmpj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mpknreyq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxzmpld.html


<!-- 参考信息 -->