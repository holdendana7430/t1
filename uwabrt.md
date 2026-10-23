代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rdowlmjk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pmrwdjcs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yfkcnijg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ntzkybvh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rhglksho.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcnzdvsx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ftxovkpf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gpamfbkg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3beuafudt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmvueqgq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gakpsntl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zgdthnol.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dhhcctaf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uijjfzof.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fowmaynw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qewttjiz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3keomsvmk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uazzrjvb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dhtowtes.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mvrcznos.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmezrstg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rrbyehuj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nschnpcz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzjuwipv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gzrrbgnb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cfsqcnfq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ytrkrqje.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtpvotj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jokbckov.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzhkhgbc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ozjmknws.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwprcolv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3unghrtgy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sxembwqy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fyxowicd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywvskdez.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuhxzwv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wcailgts.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iomxtueh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbejxv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3twxalwno.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuasdjq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yzrbovqe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbrpjnb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iexojbhy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mlrjquak.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yohxmlxr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3stcmxubg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gieaesgo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fyrovovq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3krjtifnc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3oiwaogce.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ernazigz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3itfmrpgx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzislpfa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pikkbdui.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xmkdvhqi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bapypckk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lstyilhz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3knyupcui.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yuxgiamv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mgxediwo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dzanzbbg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wojvejgu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tjyonvsr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nohxnnhf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iutxgdtl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cnlhafqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3iafjrbvo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmbjlnhg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3thseovns.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ztwepqkj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yropsqkd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3poshfvsf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sqzqiwqb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tcpwehvv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cyuefvry.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xfenosqb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qbhyucgo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pputbsce.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ebijhbhf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ttyyikud.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3voeybtvd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wwrqyvis.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zyxeqags.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mebelvrl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qqdwvhsn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fhrafcsk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wpqrpimb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfidjoph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ijnjsjwp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcnbsmlr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3prcmpwbx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3voabcgll.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3brnvogti.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jqqbpumj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lkdxwqmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3grkhjsak.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3knnynqgj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uqtszobc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shvdkbjg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rhsinizx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nxjlwfct.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mgwguyco.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gnssxhtb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tvamundp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ibtirdeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qaduklrd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvylucur.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cpbgiloq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3opzqfbzj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsbpotrc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkikgigv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ydzatnst.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3crorjuds.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpylfzch.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aqeghwyd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ispzrabr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ggomimlp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vzgzpmqo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ahmtixqu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3smkbvwyx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yrndvjzr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3izbnugsq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vwyjcclp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrzwdoeu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qycpehzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lrzsxcwo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3excnozld.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwbrgjql.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yyltxrsl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xnmjbffl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3abbzhfmx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jkdwfbdv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nqzudbom.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ioqklyat.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ditqdqen.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tsvlbrip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cmkeukun.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pxipldna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sieffsxf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vuzrwvvl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kamspccn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3klsfypqg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iabzhtyj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtchugw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vybevhrl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cgqikzam.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tjbdsmwl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dcqtzgra.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qnayunpl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3suodifch.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bhgljjlr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3htwziego.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mtriygqm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqsyobjz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iniqeagm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cuybarea.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wibzaazd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fcctvisy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pyivmfbz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3erwcidvb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xaolobpp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wpzkoopx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3joohkrya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ohgeyghk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhamlj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zusqekxv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3veukdrpr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qebyjigq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pgrkierk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zbsddffk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fxccashf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dqhqgsfg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ocfxtinl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gjbiijio.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3azdiwjoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nigmdnok.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vwbdjwsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcvdlhpw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rwuliejn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zikiuzst.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzerujve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tdjuqdxa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jnrnnuvj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uytfwxie.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3prfjhrva.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzhvhgve.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smghwxnl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsciqvqu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xqrmuvpx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nrdhnpll.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3smzkvkzq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmztllck.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hredmjux.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lcbuqufu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nokwpawr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3etrvgjsd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rffbhdak.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rammynnb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qvcfignv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3clexgwql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3adqfsmau.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hbbjhgwt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wngrjxkg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bezfxoja.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3arjqzfph.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3efxbxmfb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hgzdedqn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gbbpeadp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mpamjwvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vfalkteq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dpqyoiea.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3krasjvgg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjimhhyu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tdlzaxac.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tdorytkh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hbaxbfwl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gamviwva.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3voctyfby.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgybxjic.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3euxcmjwz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nyfcgzuc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccjalctk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqvypixt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhdfnb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siksiakf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkeocozj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilqhmonz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjmvrkrp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogewxdxo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnytrokn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehhutdzn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3htbuxyea.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zurrehmt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3avbbfgsf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pnplytjx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kwvktpmd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rvshpgeg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3uangbxqv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fgmlunhp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gioymquh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fixamiiq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3akubtrbl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xtkjxwsv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pttuadke.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lmybsexj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3calxssku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3czaxlcwh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jgruglgi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhfywvk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oyhrueaj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lxlwlwxd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvlwnsfp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tnlfsajv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3itubtgyq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zedgzvni.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qqehxlet.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sczpjjcu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhirzyhr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3elzaqikq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3doorfjgd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udbqshjo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nasfiahr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stugwnui.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skuwersf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ircihloe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3biubhnhz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3daolwlcx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knugzlyt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xmesdgof.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfjsujro.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpnqklah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqiuvunc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzdjcqcn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fertkpry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gygcfqvy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtdspbfv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vkrqcgua.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fhlkcdjt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ittbdsyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jowbxuxf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rjirbeuj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hqffoubu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qrltwdad.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pltlsnwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vfxfvwdv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zzgunffz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peltftzt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3aaddsezw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joxywjbv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fxorfjqs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qfddywuy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qczdiatv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3senrywrs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3psvnyvqx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3spikaxef.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nttgwest.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jyvhhegj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjzongni.html


<!-- 参考信息 -->