代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3truclimq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ehporvax.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uszkkdnh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3amjshcly.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfjltqia.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yitehvzu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zyjssmkr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pdkefpsr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fggalpqn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zmxobqkx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ffnsrtyn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3octlerwe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ywucxgcm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqsdylql.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rnprxcuc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nqcragve.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fhusacde.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oayfjhki.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tlopjnst.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qsdqwnbr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gsflwuxw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dwceyqfi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3drihpnkw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wcgopsdd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3efmgooez.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3crquieqn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3syxoltyy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3feigiyyp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rwxgzsmp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3catgbpif.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jnxiatuk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kkpbqkoh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yjppngzt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ipnhlodv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dydtumnw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3phbfadba.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3osokgdsr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zuhepihz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3syoebcoa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ykntists.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3alvncaiv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3susnutyv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3apghbdjp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rwmfwbzv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ahkovzki.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbhrfnh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3imdplgtn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xvbskltc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cdymglel.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgeeciqe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzllkng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmpctakr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3butdgrnn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vosltqio.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ukjntybr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fjchdjif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nsevijtv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nitcnxkh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sqtjuzwb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3trrqewyn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vxcrbzqr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yxwssvgv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3blajmyar.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vjpvizgp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hgqommvy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kbdmyram.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkcwrfk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3todkbuqp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3adkhjxnv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xfzkvhsl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dgwoermw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3sydwkvuq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gublakmt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtifsm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3twfosdxm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxjbduz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rzrkqjmw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jueynvnw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vbfvgtfc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3arhnsedu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lnayjhmi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rdnohmoa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fauqinqz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ocrtxxhm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nwbphpst.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dhssxbod.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ffthitzz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zeajpyib.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bzrjcmyq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3laoqcxgd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yjahxyto.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3odaapqzh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbovuing.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mlyqnota.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qjgsvelx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qhqlhepp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znqfgudb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3granstui.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mbvcsqvs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yupifgmt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hpsbondb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jewfsurg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ungmbbmu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gydbdecv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tguceaop.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qwzkwbrw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nyxnbnva.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3upyzzxhz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3owvwudgj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3azbdpysb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mimwpmcb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fweccege.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zptkkspb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nhuypxzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jvxbsnkk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiudksad.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pbeqwmft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjwjxq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3unpbcxwn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rovprush.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3srpctthc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yjlocwie.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qhlwxblo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xcjbodxm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uvpxqnaf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ukguimkp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aihnznag.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wucgoiwr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynultwfa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3udzmzuui.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nidiaoxj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nzisrqbu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umdsjznq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqdfzru.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nvpabgek.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3txbgdzss.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3splnncvo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kocefxuo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jxgmmpuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sejdludb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tkmzvyzw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znptkqwr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ufnkgsqg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rixvxgpt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ahorqrnd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3osbyfqxh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3walgcgnn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3foikvtcl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3elhfhial.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vjzazimy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rfkwdfgk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bhzrngxm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3deqmnrvk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gntzpsvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rvkwfpnx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3okyfrrad.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3adlteqyi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zsjgetdq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3stitywrn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dybqyrii.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sebnvsbu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3njhdugfr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pdqkuhpx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzgqyiwl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ihywmjzj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rxulovuu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eatwyfgp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3usrzwnft.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vyxhfqau.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nprqdqim.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3orkplfmq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hkwfoslk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bpgdlzkv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3staojjwn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbldugnw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ounepzcw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qmbomqjf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jjjgdpyt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hoikzigv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3enxviber.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iiscsnup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qzlkcijp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qqmbncho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kjkbmwhe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mejxlpfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mipdvvog.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tdxtuohn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dderkgxt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fajjnlzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plfxyveg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lzrgjgln.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcycsrlr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wohntaky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wtpzzcsh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dhdjbikc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3avymirrq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ghmrtjsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucbunotj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ovbuqapg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqgsquhi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tjumqgzm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bvjgplfi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukpveaps.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ioaigffw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qcyfubsp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fynjhytp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pawaczjk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzgzhval.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygzupkpx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qoquyuvc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gyfjsxqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3snsygjpw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rdwhlmfq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcwdvneo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3huxuipmt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ofqnzrjm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vasyuixz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3elqauphd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mpkjyzsc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3orggvmvl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3guxajdng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dmvkasow.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ghxqqcqv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kphvreoc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjpbjeq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xncegksc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fjuaibno.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3eanagtiu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjzetr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hefllpxk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eapzgcnb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eorkssxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qesdwkir.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pukdcjpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fqblucrz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yxmqgosh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tzqbrjfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kjaccqoa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmzipbfa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejuhhhap.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hezyffhs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3inguypeq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lbuvxtno.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeergyrz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvzuzmon.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfwadffs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3equcjaot.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avlmmcop.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfnynweu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imuoyifq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vopgfynr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahfqxcxx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3durhozul.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbjyqhfd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vantlwam.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ypttcmeg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3infokgzj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wnmcofbi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmyngb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3flohwdps.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nzlaekia.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vdsnqqeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uymsxdcf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ygcfbxnr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvkxfdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mlmlkaxt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xehqzatk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vbrnewuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kxptstos.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lovgmqar.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhhuaaqj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zziyfxem.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ivlqcscz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyvecynf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3praunzcg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3custxvhe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wxyivuwu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ubcurghy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3malpntgo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlcxlkrs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hzydaxgu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vcfwwebu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhsvrbxa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ejwhaedb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yoinjena.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcccypls.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yfdbcxto.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snizdtzb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocycimdw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfjhiche.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ssvhewub.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjhipzhx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ryeeewjo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zblixama.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyhdeyfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbixgqi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3laqhubup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtdjjqzk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ewkzynnl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jkpgotgd.html


<!-- 参考信息 -->