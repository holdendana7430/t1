代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eiimuwgo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ddqvfsjn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ulhjyzfp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fowfdcil.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zycqghsj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewrjntfv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zjnrjnwv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wshdettj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3datntyom.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sgjtaetl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zrzrjjdy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qqyhciui.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hunpecjf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3svqollcp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vaoepfcs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3orzesrar.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ldtsbdtv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ctoapiiy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvvkdrp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gewmpoij.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvegfgly.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xndartxm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mrpttthp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdbciiuw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jyougimh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3louihwxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dvxwvvmt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tvmqtmbn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqgiup.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qouqglic.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rudzhwoc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rrfdyabh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3shlnyqim.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xarwubio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ryjmtxwh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yxymdgqh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3biofihrh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rxcejqfm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tdkhxtck.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyztqasf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nnkiwnbo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3insgfiua.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gygfprvl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hodvlnkh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ofmlhyde.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zpsggxep.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sulxmjxt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pvnjfrxc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dxwsliep.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lsqdcgpj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wgpkrssm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jcxttzyg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3smkldsah.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zcqhycga.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3clwdakxo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bcsjheho.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ozluqgzh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvmfinp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3khihuveb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ivpfrguk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3evtecsqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vzpsehkt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xkqqfsve.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyvogwap.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yfmpvcrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sifqxhzd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcwxoeze.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdzawag.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhyujhtx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bifawcrj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qymdlvsi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jdmeuxxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gfwsyzgu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3urfclpya.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tiksvpie.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dsvlmizw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wjxgzfly.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etexygnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3enmuewvi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gatqgqml.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptfbjcpv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mxlbufwf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uuhmlcoc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvhxkzpm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oicbzvyy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3twzvzdvx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iqtnhmwa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eapjkgbb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aqfmzfni.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sdwxmiuv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mqqzaqxf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3obeovlva.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zlcynvme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqjhbc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jykptgrb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3giopoadh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cnwxzisw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ciygdrag.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nxvdrpok.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bxdroevq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kfpcnoxu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mrbkpepa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wjcrejjj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jftopugf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ooyxduts.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nekfcdov.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lwjoxquc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mocouzqr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jgalkxpk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3whdfldkv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ebyyfbne.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pgcnztya.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cqibvhwi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3crdfwzvl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrbbitvn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mxnxfwuv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wsksefzq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mgzsvtnh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eizxsach.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gzqfkpjo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lrrifygd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ompqfqsn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ryvbnweq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ovevqawp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3umokzxet.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3htofmkkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhzedxdi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qxkacdhr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vdhlfqzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rnadhhre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3grokqpkt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rkteufuf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3voolztrq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3imncnuqt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kkmireop.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zrmzauly.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fvnojjpy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zetvnrou.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wlsbjiuc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lpkoegkh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cjmxdklx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ffbrxjku.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nvejgvrw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3svinfznb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tvfukjsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnkvynmg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3txezaxdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whwaeciw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdlovcfj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zyzvnyno.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nrwreclq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rjpxdxwf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wtcspwjb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kbpjxked.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ftprqnyw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdryincq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rurkxzmy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3udwdtyfw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lsfbimdq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3msoenbbj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3infoqtow.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hnqegquu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rgrilrkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3crimjujv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wfteumhw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3seajagwa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3muzkkouw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qokpxmrx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sagkzrzu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aevnwejc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eyteladr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xkouxfob.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3abclwhcn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ytfzkgvp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3znaoouoh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nuazpgbm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xybxavad.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cskluqwu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3khkhfgfr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pqqvcvav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gevslcrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pukfnjhz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bdgzhoma.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gzglzwkj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iiuhswnj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xozlfutc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrfbfhfw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3geamgbgh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvwygipv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksbxtwjn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbiramv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niqiqtbw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jegqabpr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yenpdssu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gijbczhg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dxiisqca.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgbelvpt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkggniwq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vevctcxw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agdiemaf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwqzafk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fdmgwqtf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zomyyxzj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjyxgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sjpfjnbo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fjlcpcvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ohxveyae.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xfdiigxz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nduohpwp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkkxds.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wwvlnqar.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wcqyyocs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ikdgebfg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kummsdml.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3veaiepgi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vfhumvtb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwtgjnm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wxmaqhql.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bdguqyrs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnsdgrgu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hpygvwng.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yquplcph.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3knfoasox.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jobquuxs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jpakoefa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oxeakzil.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bmjojaau.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvaxgkyl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bhmkauqh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qjpcfbhw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpgoacge.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iqvcwttq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mssdctew.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmulwyrl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bjyramxv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmfbfphk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbqyrrzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhydltaq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3facxyzfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nryyctyz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cvgqozzn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3slurqhgh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqtyxhe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3opzhtneq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pabawtid.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vshmlhjj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oftxabrw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dplnqsrh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnoefgs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yxxtzjtv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yyvrioyc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3nlihcvof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eyxktlxh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3evahhfny.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lpchpmwk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3arlhrctk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfdrqwrp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ofnglmoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eabnwjyu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rgdffcqs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vwytzbpx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ejzpdyaj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thxqmfau.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3iummytyo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zcbeeerq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzjgtun.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qvkbmmoo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrgzwcwn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vpewfuym.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gtrzvhck.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3upvjkxhk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvtjdtga.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csiqdulc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vgylqzdk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ztpztvuf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yasycibf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhcpjuy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rqjahhgz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ijtxjhyx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iahqrxzb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ylpviscz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wyllyxag.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qootqubx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gwomodso.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fgtmdfqd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jedlbjru.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gcjbkbls.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3twczejhx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdipwhzo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yebsnxqx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxpjonz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwpaidpw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3raugqcvn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3redoetgt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3skbwidrh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dedvynoc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bwyitdws.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3knejqviw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zncccjid.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kmypfuug.html


<!-- 参考信息 -->