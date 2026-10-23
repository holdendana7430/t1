代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3eithvqfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3znmfdpmu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3isnffevm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpaowzeo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jclaprdz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fwmkqwst.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fcofyabk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xcnyndpg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqzlux.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zqwsicut.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3huwrnbug.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzonvndv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wbzirxvk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zsodultl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uxheensu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3acnwnxnx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mbkynosi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3baxjeufs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yraezvwp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cnznrdmg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3visdrucf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkqaduc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fxicxlug.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hlnoomwg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jnfbwadt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufeygize.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ojogthgx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqluvmgu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cubiusbu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bxogiwwn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mgssbfzm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ijmnmkuv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lsnovlhd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3byylhvxl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lzowdlqw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mcsbqmrp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3adojxjho.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wpzraudz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkuznahl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3exlksqyh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hlvcccyc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ievudtfm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tuhffeif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bgifdrcl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3iufzovcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nxdrtyze.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hjcwluvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqopkiz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvzcmkhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hscdosck.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ekriuskw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3libuzfxg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ajxvoaul.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bjhrcsop.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yllsbduh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jzuzvdqh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hcohwndq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hynkjkkx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3egpxheyp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ueldelow.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3owbzwkty.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdtbkul.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jaxcajrh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3megyfznn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vwdwnuva.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xlwhupmd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3glrockzb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3grpcxgac.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dumqnufg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bydozbvo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uychmjph.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bfjbaanh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tvjtajxk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hrlawigy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdejyhx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qxbtvqkt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvqsgbs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3efntiffu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nrslbbze.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iznwitya.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hkwsmvkk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3edmaextn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3naspwpsy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ejfdkdly.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gurcrklo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kovlphll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rewumqui.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjvhagii.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rsmkamso.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knbodlet.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3anjnsgvp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mjupgkri.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hyqwytog.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fqknxgta.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3oinaiuvs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sdnftely.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3akmxscum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hboxbuzl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3asnpjljw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xncfqheh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rwzwlfcx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vvxlfeob.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wuhlnmra.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3syyjrxxb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3presfqjd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hhtaeqdg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3csunbvwq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkcuojqg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qdwnbubg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhuupie.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uhzzerbe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfzbrpm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cueebcfn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qtvyglim.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3prohuecs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnihugzb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wvspfthx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oejhhvfk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3afmitqxm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rdfuhfmp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhyayqa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3irbojbxi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sgdvozdc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ceogkdur.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3siaaabls.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fwphwhfz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rrsligon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3conrrvit.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3leoksdjn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxzloqxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ukypizof.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntojglhb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yxesrzoz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wodrsiwq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fbfwvwxi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bgdmwfuv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pjtyhtmx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kwgbcutf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3waadftrh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yexthkdc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mlhuptou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pfnnyspw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qbummire.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ymgkebmk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vdwkbdul.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3btkqlgsq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhqqaft.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmloalsv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyakigzz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3najwrzyu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ncjvpdmi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mfciuyyh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3braupkvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3izjkxecf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pgwtalfs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jobcyicn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cpagnhag.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lrrryedz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yascsrns.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bqwacfeu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vllxwxfn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hncjsrkc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3unzmhosz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mttmbweu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3joeoqasn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qmkzohjx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwxwfor.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3spvuvcgw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ukjdotmc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aollncoy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ldyxasgq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gsrhpbfr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3iosjawkz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3efnqatdb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbsuaqcy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfjmwmxp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lswyfikr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yliteeen.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jdkmnphk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qsocejxp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fohruqyg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xgcnjyrj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tcttzazb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rffrgvbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3twdeuzod.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hhjxmnwd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tlaljmrt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xqqrsaeu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ktcxheeh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3oynpzaym.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jqideujr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qosclrrv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dplewlty.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pnwkwotd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3aehzwtuh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oflgydcs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3adwaaopa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfmoeyqh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3viiwqamp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywfioiff.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3vmculrgv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xkfhqpxq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dwsohrwc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jbeqmtay.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3orapittu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mbpgixlt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dccnxcbq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtajgscd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oqftyhca.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrnuby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wiaxnpyu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3natfkkvn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbgessva.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyevfwkp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lddlafdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3avfebmmz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uagkgzzh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3njmknovo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jqgklpnr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3amombwra.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tdrtrrvr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hbjtbvpv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oavzgcpk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zutvgyfw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wzyviuoo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vltrdyma.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eeuwpwtl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsotrkej.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kgqgyafo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwwbbnh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bkddkrfq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lesbstri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ziodlkov.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rjhwbkny.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxcwuou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xrqyecho.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rixrxoek.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lbzcnloc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbjbwsfx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swdupovd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tylysljt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cccynijd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jgelcxfo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aenhzybn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcktrvch.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3decevrbd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyalxreb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mouslgof.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgxlzlav.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqyqbhwj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rgcohswt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfwxbltw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfvqqiir.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vigwslix.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ngjupioa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mwaxrgji.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rkurribd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nyxmbxid.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xftwcacx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfukfvdo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3styrblyi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mzdgcpru.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rivxakci.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vslcimgm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3shardsma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zekbruyy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zzysgocw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nciyvojt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3atuiugzb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cgmhadgp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3otxpqatv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pmshzqyd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cgkrygsg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmpannjh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwdiohar.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3otvirfnv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vutdeqvd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqobwakd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zbqennat.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbpesexl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3crnpyktg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hrmfrrut.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcmmukqa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cxtpqnye.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imzcross.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcuxdmfh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dvqmsype.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syeaqbwu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unrqaxne.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndupgtuw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3aegwyvjx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijlquyyu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gezbprqh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpudvifk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydtovowg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rydmkwxy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gcieendv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtiedcsd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nkdjbwsx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mvdebwmj.html


<!-- 参考信息 -->