代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ktvdyuxz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qegankjw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3trzvgwkk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sjglubth.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sfnnlzfw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eyalclxo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yjnytinh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gqshilvy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zsvpgdjy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jkfrtnkn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dsjnhoat.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qyaecfcn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qofrwaox.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dqkvxtou.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zukgsjir.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qnlsqmhu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hxklmqxa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkbmgsv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ekrbvkhz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mipjdgwv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3znsnklop.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdvhmi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tdktbkvs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qdlidnhf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ojordfrk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ikqzeats.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyhputci.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3alrsdbnm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3epcxuvib.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dzagqaoh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pbskyfhx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bsgzxcqb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ekaxgbzn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yovnfrzo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ljcepatj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ujicgcal.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fretrkfv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mujryrgt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gplmappg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jrukscou.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3viosuhwg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aizuphyf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3piofmuan.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ucyuubbt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3oefeimsk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcesecas.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3facdjbdb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3scrhjliu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnrbfrsh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3irpyzlbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3woyvqhnl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkddrspv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zsxhuxzq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3enydoksn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjiuzev.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjxiwkg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrvhrzf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yriojuip.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qqbzfvwj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xtrfisoa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jtsepxhh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zindhugq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksyjsoja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3osdsptzz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fufrdzla.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zkgckhfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ngxlacbv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lpifiqoa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elyetunc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ysdntogc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3siodtwkg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfyxzqbq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbmfsty.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rvbuykww.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pvummokc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yqevkedg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxijwb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dhdvdjhm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3oebowppv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ehxwhpbv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3blflljmc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmiywiln.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmivbce.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouhbiitu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sftsbiwr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jcqdprsl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vokhmsfn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3oqamvtqs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ptxcbboh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xdtafbgo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mtnkfngj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvowigr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vuilaeoc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ozewshbl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gixzwxna.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ttpflfhv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrhbcckl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ivutnfhh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tfkfvlyh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wmohgesc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yytfxjjb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3csgxjmqr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cfcqektn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ikkuzbou.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jgxvvqtl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hdletybk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3byvkbsvq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zxdgenom.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3evimkart.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgcjiyso.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3sszirlaa.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wffyvzjb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbulbceg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zrifqkmb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sedyatvf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ulgmiihf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rnihqzhk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qkfscwns.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eestzuro.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qbzlhunx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wupxerax.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iyhvwnhg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lxqlxhdv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nacvpimi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dtzwwixi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nxqhahxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iszbappk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vsiwltbb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wztudieg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrafztr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zknhilun.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cetafkkm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqbcqhua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpwsoari.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ejmmmmbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhshvtbz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3afjwjqgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pmztdqeg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whdudvha.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cvauuebw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jddazflo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3paqpfdrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3olarbgel.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqnkwpvj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lemngcmr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3yeoypqvj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3emvmomlg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iorfhoyo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rfmwtsvc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ktcirjav.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eckclgrm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3znieroer.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jjoewmaz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3waibksfb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gsyqnxno.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pscoxjev.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3skqgfwcr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3narvukba.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jjagqzbi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hvjqesut.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dkiizsqj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cbotjnhq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qcvnpkiu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oxitlsgc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dbfiseod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ujbzftbi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3turwkvel.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wsedqbyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lxhdojsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ontoxvfr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dgepwget.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qsyzsdiq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zsltovlq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3reppvkrt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yoeqegqx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3miviydey.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhbbwswy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ryekzmyj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3keilenmt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3annmnqte.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oaasqihj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjhtjgpu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tottknvc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqcqqjkf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxfgkeas.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgjunxqq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3untmsxop.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwzodg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqyvewtt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwlzupcz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wsixqgtj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mdsjgmty.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ovrdwoia.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gblledha.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cfeahpdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3alaiqeum.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fippmdzb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3brdgxkmb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3khilvoyy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ctzqjjyr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkchkmx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajeoxvwj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oovrmhas.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jvqpjvkv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3moaceohu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdbmgxtf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3utnguuzd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xswuyiyh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fsnrazuh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tltydghu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azszvyam.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wvxovcjg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yfqwugog.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hmtqinfi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jcelqbql.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3htnwjyyv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3obrdkljh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3clyyhuhr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twxrzxpj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dksjzthh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfakouce.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulqlmutg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gjgcmuvx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qffmknrf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdphstcj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjthiwrr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvpoqzhg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgkqtjyv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmnsprxc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czzpwdfj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvkshnzx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsftqgh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fkeqvvho.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmtjnhu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cfrngavu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vkgwuvqd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oakwtwyh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jovszuzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tdndfjcn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3diqdepwf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nktutlml.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3icwnvcyh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zxmsvogw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ympssuca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odyuuzvr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hytwfisy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsloyfby.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jcalhnac.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3seuyworc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqsfleqh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsoxavnh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jrabtlqw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tcpxtngl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mqddyuaa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lfufqahj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gunpxnbz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3efkreecf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wsbdslic.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3spgmvpvt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yhgsxvhc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aczqorfr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xkpwwpfh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qxukiche.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3goxxiefw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wdpcetpc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qpsfnrmb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ratcrwqg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3orhmqqwv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yzkisjxo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sxobtvwy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ciakrgjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ovplshxj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eloueqsm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xwmbkpgd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lgavkwqp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wsgxoudb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayzhsspu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gttbhqar.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irajtyxe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kplbllvl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uocujvop.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hriduzjp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ddqzuczr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgupwj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qpfnamwh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpgakxbf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxhtfvou.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3naxiucax.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzzuul.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gkurycoo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mhxnwabx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3loytghkt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ptszbffl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3duqxyrox.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mpckexuc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3munamzdv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tymidvuf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiriqxns.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zbjttfci.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3czmqowtz.html


<!-- 参考信息 -->