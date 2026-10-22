代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yhnvvjad.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lgqtwblz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhdaluaz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lqbspkvj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xkasprek.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dadpofpf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2plmqwamh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2azwdpurh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2peonbrix.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ospqjhgp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gayfoqhj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iiatitsd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxihslg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2amdvmedo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxyfcxzh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xozqwrug.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uqajmdwk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2khsivdea.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wzrxhuur.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ptfnjtql.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ywfocvmr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sqbrwnim.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bsefvwlw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jjauukwz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ibbdmbdb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dqeboqis.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mjgmngyh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tvcvcyec.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjlsclg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mumqfpht.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sdkvxkaj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pyynsfll.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkkgseu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovoosvmi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tmxczgvj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mmeiudtb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2whmxdlqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xpvpmvtn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ktphikog.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lliuufga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2elyavjvr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2whzxigcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zjryxgkw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2scvxrwkx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqwkod.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vewuytuj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nzbgfxzs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mebmxllv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2piydziel.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vciapmcl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rhsqmhrg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rhxddddm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxnvlryu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yeslbgiw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qpfghouq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2portvkqi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2eazzdqok.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iajgmwgo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqwtpqsf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jucfkxyt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dalzkgag.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yxafrfjd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jumjjxjo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ytxkzfzm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tlfzzfir.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vtbovhdv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmuoscoe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2daohignq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljcijrii.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2akmpycqf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wntupkei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xogxieww.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kvncyeun.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rehkmbnf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwphhvvy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2phiakwiu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2stlsgvte.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wxsbpmcu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2sdkndtqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tisxkpbv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2stzrjxoy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mganfehl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zehgedwd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vkbuiajf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uivyishh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qmfnhuny.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wceyjovw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2iadtppaw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rydvueat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ukqribeg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghmqrirl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kemjpfus.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lcarfqtf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ewtpubfl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fcriyplg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ltgvqxkp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjkaqfjy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gveuvkjv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yicfsbhx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2txczrwry.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vpfljfxk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sjbgwrjk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pgdhsqsq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djstzkwx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rserhpud.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pqvsjqke.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yfgkpbrv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lsobdscj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bvqanppw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2euakieav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2touetubt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uulqtfnp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bpbvsmtm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2adcislgj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kqamkasa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmfkgdku.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ucmkjpej.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2egpezfsv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dnahstfh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dzqchqjd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sonbpumf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wqyoakij.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rewmrljp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfqhzyc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2geqpghti.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2seyomlyr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uvwynwtd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qdnxdhex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ozoncekt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fesmomtf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2svyljejz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyvwwweb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2utpqadxb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rwqnkoxg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uglvnzar.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qizjsvuz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bittlxpl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2awrqxpmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bospupbw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bujqutep.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2finolvij.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dmdedxqh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cgubprjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kizadhle.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ephpwbyw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyncedqk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2etxqxtze.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kmxubzaa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ogwhylsu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fdbexozq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mxjlmakt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jfgwympa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kqknydkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udikbndf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nwpjlxah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqqxvcqx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2thbzshnq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nfimasel.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxuyvwew.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vpareoja.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fvpukrrt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2isqwplxw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xnptxbip.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abyfzndo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ujnpjaly.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyezmzln.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kiucxojl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nueqdqdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2likcmqod.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lorykzlb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zcmwbzgg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jzvijjab.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fmfckcga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tszpozhr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hndywbwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cxlxrair.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2islbvvby.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lotigjhq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jaoaycio.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yhkucwvk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qeyizbpq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hskijzdt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gltblbaf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uvjydjal.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xtgnpkpe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bmhwbayc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2faxlojqc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wpatygmh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tdpbrato.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ihkgkvbf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2epjsirhl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vscgfkgq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lyzeoipl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lwhseiit.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wzhnbxls.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvjzpdsy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znfymfrp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmylsnru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vqgoyesr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsurjwpb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gujnrdda.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zmzxhfns.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rledbogt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2foqdnlgy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thmdvodv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilstfzdw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tlupeaot.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmtenoon.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doezcavs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wohgzqld.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zedbsxfw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aqtrrgco.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hqwlezdu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kxwuldxd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cegvfphp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2iiaqlrht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtpzwpq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bhafkdgz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2teowbhzu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nfcgxlmp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfruwfu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nklydgzp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jzybsslo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qpjibdzv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dlxjjwuq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lgegyedn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkcbnowk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ejwjvbal.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2szmeybkb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eiwnmckj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oivxnbcp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kztbibro.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tjsstjzh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuogmftb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nfzlqrvi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnsqoobv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cokzpdou.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nqqezrks.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfvimtos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fobdejlt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxhtpgaz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sedvcfeh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2plmlsozx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auyzgtuu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcenidpk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnrcbajd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bcedbitj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozrswbvh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2efbqedvw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjqohysk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owdurbwa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dxleknvs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zfmfxedr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kiwpqhfl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2imxcapxe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2znvmowcn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvmvofb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wsfnkujd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rdpcgwoc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wodkbcyj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yotulzrk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qqyagufu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gktupowf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uutmvrtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hajktlgs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dsjgrdss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwuucctb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uwmnnovv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2aezkleql.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jinapswm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mjwcknyz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hkxlriim.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lujpaluo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cokuqkwa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ounznqbi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gbhguzey.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mukmtnux.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uecflipa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfepoqrp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijcvvelc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aybunwqe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2puxhxwex.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yhtalmbl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxyftnjc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2czmvjtnb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ovzjfonu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ayyeehwv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fbcmkigz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2emujyvte.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2thkpqtzf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dcaymzco.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ovajfzuj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gcpkscav.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojeexssv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rdyebbuh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2juawuong.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vfoqqzqy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mkpkbdus.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjbzllh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jplaqsph.html


<!-- 参考信息 -->