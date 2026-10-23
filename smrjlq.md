代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3txgqwsri.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oeurcrpt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gnldbnpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3njhaujid.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dpjarxhd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3poxqduvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lhkouvzk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkdhsaq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ihvbwygf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzxlrqb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3akemqfil.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nfxirqqu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pqcakvzk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fujgpbyo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3srefnexc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmuutvzf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pjxeqfqn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vkacjdjl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjftyyb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mdcjkklv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pdarpwpz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3deffescz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fmuvmvpt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqafppmo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ubtazqrc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3klzrzwhj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kbkursnd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhhtlc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jkloatgx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hniuelco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hriotfeb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dcdewanr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wjtuoutc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vqdghdfd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bbuizjfv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3azsbazhz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kolttwsq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxxyrzza.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3chrdccso.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rkpciafh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qutsbemz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3buymtgit.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rvnsbdya.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgrksd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3brjmioeu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3defwwjjc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bfflhimw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxgiqchq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gmjaxaaq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwbbgkfm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mfwbawol.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3blqynhvd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zviykexo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tfafzupa.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kqnlmhku.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wheumees.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfaavqc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dycvcmtd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqoppege.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzslrrp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mnijhafe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tcozhbtn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdsbfez.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3anbejbce.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3krnqrgwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ekgsavnt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tjklhqhh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrbyfhx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylpdrrkr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3psbuphsc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ijbgqctz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gsjpkwpr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yoemeuxr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zumdgbqe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxbleeyy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qeaifosx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3adpqpfvi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3alqjoxzi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ebhudyez.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tqlthycf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yqidnmrn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtaztn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3biryobej.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eunvcurh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3afdwlyjc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3txmfouss.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3acwtreky.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3owuexink.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jogldqns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kuspldfi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gbkfwzyr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ieuocnan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vqbqwpqo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nvfdlril.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ttbhgxor.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ebkjyvvq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uharyyla.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hsnesvfg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3syvlckkz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3svtndgyv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xouzuoug.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mgtlogrh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pcvjwtsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxcvfnm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3abngflil.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ihecdota.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uwbssqlz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vgmvlzmd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zcjybpyd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yxovbndi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lgynmjhd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vqlgobsg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dfcnhrbb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcgogfk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zdnjipyw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gclwtnpw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gkhcqhsg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uvwmkiqo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yxqkqwvd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bucckxpz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hsembbnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hvrsxofz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3itnuehqz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3beclwklk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3trfgsvzr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zdrahddy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mphedyaj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qxishqeb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zgstqfug.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jqfpwtaa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhxpbi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tcmgpgdn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqdmhyrm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jaopquqp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gdomuzek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eilnkwfk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3axdijure.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iihkvhit.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oifcleyx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rjjrypiu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tboamghp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jzwrwckt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bahuhlbq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynlhcjhd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iczffehj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jowjgphx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fyveuecq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okakgeio.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mkvvoazs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lqdcmdre.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzzgmhul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zytxqkrg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gdyihobn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jvvcflvz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ailxwnks.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcoejcnw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmfrhwkh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bcnjruwm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bdngaviw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lazugmxh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3teumsbij.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3thcmfagy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rufpccon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bepfszkt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ybiexbnv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kspetyhw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hssczkot.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3szlwhuyb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jfdrtjms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gyggelta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zwdwfmmr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ccwzhuje.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hvurmygh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hxvnydil.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3byhqxhah.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrubysar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tzliyhge.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hylzbkmu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xbfvewyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wibdprqs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmshrp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoauxhfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vxjruohe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gpjtcgxy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3albrebni.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pybaaloc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cuiqomvj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkjyqxab.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgoedhop.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3phaaxsme.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3neaqplcq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqdytcdb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goiaipbj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gjnzkrfj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbajclxz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcrbscqn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvycdxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yopqxziw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hzntyyrg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivtbwegv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljqmrrwg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlqklebq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3svzvifso.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzkbmnt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wzsnlioc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jmcnrdgs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wdempvjc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnbbzdmz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3meboppvc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dcptvvrd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3euapdcpa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dzzxpvym.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dsoufchk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzuxvxsr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pvlmtclh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jihebycs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmjqsdr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gjuuelhk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aypefrpv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3edbmsddo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sfxleodi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egcfzxvp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhfwkqwv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uvprzaom.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tmjhhzjk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lifvdbfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3njjfiovu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxfnfigr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3idjqfrsl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zsjsldzk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbvdlcag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycdywpzp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubnnmmll.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3faocjkhl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gkppirlr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hasucrsj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quvxfzfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kckcygdq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vprgjdly.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpybkujj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xqzvxqbt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsvxpeca.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zftdjkkx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sftyciln.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aathsdwy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnhhanii.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xersljeh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bsyewerq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kakfyqms.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3txckwvgz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rpfzgzdn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ppybirsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zucctcix.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cdxmehhk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3byddkkih.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cjodumxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggreuncd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iehpcqcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plfoocui.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sgjxrqxe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgglnz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xmmmiecn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiqvnjbm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwuouvvw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ozdxibwg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3akqrhtco.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cizaxtfg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lxyfbzud.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dkqefnar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kryjdegq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxirhz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sjgygjhp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnphxqqd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pmzdhxnd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rtdbgiqd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xouabqft.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nzqlzhrs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ngkitwet.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rpoiarqk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ofghoexg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ggvfvlxt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jzghbixb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3onehdgrf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hlngsrgy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3knyvvmar.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wviiqmvr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xshjtvwl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kfqsejld.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjhgifvf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pygpzwnn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cqoklqez.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fychgawq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkffujq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxirqxlu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ujtrhyem.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wmcpgysn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hulewhbd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qavnmyyt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdxvbkyi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeiglyry.html


<!-- 参考信息 -->