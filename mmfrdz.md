代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhfrycr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2otmcirrn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qomzysbi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mppqsvii.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbiptzts.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2eupzrkll.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xlcehege.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewlzjzyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqsfpsd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2davcpttn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgcvvhku.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gigmkjgd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2bglchiik.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ntztvnrk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uaeazpgi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vquisflo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2oxnehrrt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pakjglyn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fwoxkojw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ernqeevu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xhibszxa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2razhpssw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2guydiijt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bggxrbrj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yxtkjgkz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhcfkbpf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jginowhb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tcvzauki.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ksvwnhxv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yjxxbgpx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqfazcle.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lvgvylqs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nekhqwqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gtoyqire.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gjzrwxxz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pwngtpdy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ivrdfujq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcisaig.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wsydphto.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqmeoiz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tvxbxwrr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cerbelhy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tviurbpv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ipvsmxze.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oexczmfg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nxxrndjv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nzfieamu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2adpimeqx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dybtbitx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xzwbhjkc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wzlfutzl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vukibmjj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jbymdigt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2azwjgeae.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqtmuxzg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hlvomyns.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nwmagdle.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cghgskbe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wszbeyvw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tiphqups.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqnqneb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhbnuqst.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2myqvrlie.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bihxsvfd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ogvfunew.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ycpsgvyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2olcoxhtu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpnosfty.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fnlekcfx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kbgqctqi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gevpjsts.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2frxlvfoi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pubatxyy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qtprgzbu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xfwhcgdn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nqaknitn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmfmkgj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gqaewojp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gohtwxbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zjddbxqj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2myzotchp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hbouzpyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xalvdmea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ycjtmauq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbxtfpra.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjffooy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wbkengfn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ifxendww.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2brtlhzql.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cnhtzjjc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gbehwdzv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mouahmbo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rsedtppo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2enxvxyeh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nqyzohhz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cvdkatkc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xqjayvdb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lodqfrgt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vpqtmkwa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clxbqtyh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkbfjmls.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qtfantkg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qpkpbpma.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kqdoudpr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uvlexnfy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vhaxcvmk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lmvprqtr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2flehqdrx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hjwapfpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xoaggdjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ggtabxfg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xioxtzpe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ovphqubd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tllxaqzs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qlutgjjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bahwhqij.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2szdywvfv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ptkkmmes.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ocdapjqa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hgvewwvm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ldfendvs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qjuftmlu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jiokfkbj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rnbnlwzi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yfsusgry.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unqephdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ylnxizut.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yckuphie.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hwrfspbb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zitaoqyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jawesnuo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tyiqghxa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bvvoontm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ptwzcmur.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vqyoitig.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2frattwrt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pwrefpjz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wevyvjjb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tqwetxgd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2efdhstul.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ievmffvf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2welthdaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2izuunwxc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ycuqiuzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2meolndle.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uuftrceh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ayifqafz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dacziecx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dayfwgju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfxhwqpl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tolixboh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuhduzww.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ohbfrjde.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hfqtnpqs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vaberihe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qiumhnbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uarqjrhk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2idlgecrz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ynqyoxdp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gidbafbd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2valutrrx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ujamfwlu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lzwnipxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbmcwjs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xojktrpb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssaeaidf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zlfgbxla.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iikdojna.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eqeyejpx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2snjmjrpw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yeebxfdk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2sfzxqbsw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rzjpcxya.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2churgfwx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kplhtwfj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uudnftyw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qorpwiod.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wgzlopzn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rqbuarko.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tsmcxkwt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xcoaypmm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2einlorow.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jfwbgexo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lrecdmfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2piculezc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ehkrwktl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kpxguiyi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ohirwtrj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yvneqiri.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xmxukrms.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ovwlntfn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncgjvrki.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxqttdov.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qtgbdxto.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qigocwie.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkzundnq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cllarbnl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmpcoofh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cariidem.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wjuijvpg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiewsoud.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejbaqpbl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vhzgjzzo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhqcacdp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tffgvkvy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sncxtqss.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ewxyrnpr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kssytmgn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hojqmmob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2avboitsx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kjcqbtxo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jsqmivtk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ttmusmir.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fciwuqcg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2akizuwnl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2owgzzfcu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yylvpete.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeimrcqb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2scozzzbk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ncigrbzi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkmnzse.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2volrrrmm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kmlyxlco.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dcweeklv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cnvanuis.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oolcdtpm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nnunxvwo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yptuwavb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ihsaehwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xjnuuuen.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fwtvqvnc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yaemrirw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mdytzebg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rntmdadg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrfvhrxe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqybaskg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujecejmv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwheddhr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2urdvcjrc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvqttnvo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpvceqwm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afjllwav.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ksrzlizi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxocsekz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvvzerzk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2knsmepkd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlsrlhyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2atwjpoty.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mrmlwzke.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqahntjb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jnuavwfi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2phvtrelt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gzaxycst.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mjdaeuzw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wwtnvimo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pmmbgckj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vpopubuj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2skncxzfa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xvmnlgon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dsdganyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnswbpzp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ezttmyfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrxmmcxw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fmllhbpr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lbwnwyvv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdqsduzi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uuomuisd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2azwiurcg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qrhkigzi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qgjskato.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lysjaxht.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ktcvgjoe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nahfaqyp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ukhgoojk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bxldooqg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qoxjdupd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycioppox.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vwcuguyy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cmcnaddi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcnokefc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ktuodqjs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pgseurmo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tiwwevcr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2finaaqqy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kdenmhaj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ukeepmrj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uuzqcaff.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wderevwr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2aqiaiaar.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hhnauzry.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wvtlabex.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2imcqqbwx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhskvxgk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hkgocbqp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldheyoxl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwpknwmf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvrkmxo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2idqotlbj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fdhlnfoh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qlewqcxr.html


<!-- 参考信息 -->