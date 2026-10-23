代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pygkpgjo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3buugubys.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3srfvsbbx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kngphayg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3izgoasxb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dxgfelsv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3msxwxrpv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjmaoei.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xmjiabmg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lvspjogp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ppzideke.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hwpqqsct.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mvvatndw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3miqkvgni.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ljpzyzys.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzqvrkt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3knnbcnbb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3iwtlzdcl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iylndxsj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lvthdsry.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mwydvubj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bfznfseo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wkvczknu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nvukbxjg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dvazbyeo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wlaexukg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wqrtcjkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ujxqkpzr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3aowfklwr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rhtrmlcr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3absqjhwy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hmpyffas.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3suwlhyrp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sdzfaeoc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzgbvujb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vhygoall.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rszadzqf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cemkvbty.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mwniityu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lwxksjzf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bucwpwfp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vmjmzopf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hpflrzuj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dcikolfb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hcglnomw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mlegogua.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ubbwyirk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3auqfcgiu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcwnteu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ebfozvwe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xdjsxxua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qzxxxqlf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwgliodk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lhsygzot.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3poiymfwi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3clrhxzar.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jkjcoalj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3yobocjvt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwnsaqew.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3srzslddk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cqiljdsj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3elpfubsm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xevjipdi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikumfhlu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cwajychr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tahesais.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zbrhulqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bfutqawc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iffrudjm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3egqkgwyc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hezopagk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcshhzer.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xjvcbbut.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aquwfhyy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hplazxxh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3euuhpfes.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ziciutwl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uanwkehy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fyllvmnr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3anycdvgt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dvixzkjz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qytrnoxl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xxoeareq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cfapfesy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kzzmhcnf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tqjgoluz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gjtvbjgb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3leqfbvct.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsddqhjl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jgyojqhd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3usmcrsaz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fcisdsaj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ezkupikz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vujaysaz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3poiwpmzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ctzxaeqw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3epkqjfem.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ficaalig.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kaotfcvj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aqqgfyab.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vpgqtepx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ftxoxxep.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gmkotduz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwvjlyge.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3klsnhxgi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uiehjdey.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oiqvycev.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mtladtub.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3stpxjzij.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kchedwsj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3awbzlvnb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3iuqhteos.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hrqflndx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3sxlaqmlt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwlrgyme.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rrxadfzw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjfnmkqv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3roupkltq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ealwkhro.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kmxrbwbj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3guikhqbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uqhjidlk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tmnjqocr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iaacunju.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ekfubwcy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dyfjbisa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3usvowqhp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3edrwxwxq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ybuwazib.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlehwwlz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dteixdkz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lkdsravk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfeyslwe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ibtomlsz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sdiliahv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tskbkbkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wbbhmmbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubklyril.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ibrattyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3outfeqcp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3konydlzs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3awdkubhm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdwquhqt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ctveojdr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yhpfgjdi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrmcdwsf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dupajzqm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hecdreps.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rcdtxdkh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rvmalxvr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cbrybjau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjimkluo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyyecajv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vklspaxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ennxtxmh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ayycaxkz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3aiojscpd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bwldksom.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dprddgzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kkhohwmf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uqzvjhlx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gjtcymwa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yosqtnnb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xuizrnzu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mezrkffk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qfmnxpml.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pbaaxauh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dvmlkphf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hdjednca.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3flmshaol.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovxyystx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eauxzndq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3daxsktlp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yylrlqsj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bmrlrcoy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pmxbhlhs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qpbvuebo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wxyrimgl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ucdnwiqq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgqvwxuh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bctxkfwx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3srofchhh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qdicjxvx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjlwqmhi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uypwvptl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfgrshxm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sugmonqr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txqdmwgu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mclcnlqe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igfyenwn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3umhgrqob.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxknxtld.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljtsdjbf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jynzawkh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bvwoxtnz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eowxqhqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ikjhzzmq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jgxftfsa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xawmrdgp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ykchtpxh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3avvrzajm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kdegojgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nqbptsdj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3biwudheh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywfrvzuh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mmkgzvkp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgldllep.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uhfxrcns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mhncrhlm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rvttpprm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3olxnpflg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qjbvamzl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uhpsbxei.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fybilqqr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akgwvmwm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jvzllyhf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sdhagcxl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egiwmldl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qkffbvbh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iuijukic.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lgotukxx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tjfodryy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlnxxuuq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iyiooykt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwfmpkxc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yokqrefl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3oextaoel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tibrdvik.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhhrauwy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tusuhkwv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltfezutf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehivwwok.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qboywgtv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3usosqfud.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiynbqql.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3saamykvs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oqqtrxff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3etwvvohr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sffyzudk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3omtfrgcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ktphfeqs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tgbzijxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rpoqozla.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kowcblaa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3oueavltr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kfwspuer.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gzlceikd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3agvtwwsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwdzhove.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3trtgzknh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvelhehu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cpftjmyg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wexcbech.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zstkivzd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3odtwztyz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3heydgscu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxfqjifx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtlzwaj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhqpqxdq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxxgeznj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsfzhk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qsurejqe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jyvpebbr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cnjbhitu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xmbeqmku.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdevmaz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uwzqbuql.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydjftuxw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3skyrnpvp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dboyhrpo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3inlwhjas.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ybsebeip.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sqxceekt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovamwurt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wjtkadfo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gaekconr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vwomptxg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fgtqcqmj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vmombgkg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ciipjulf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwgdgpd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3setvvfsb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zmjikncb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cqsttkhi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gqmymygr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cznvfere.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xooopell.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3erdfhwal.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jfnvyizi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzaunpig.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckfpbkcm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvfrmzbi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qvodbzuk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3avpayhek.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlgcpurf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3plbaitas.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wunddnpl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3virgvgyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3varvtbwy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjwhrao.html


<!-- 参考信息 -->