代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uhtwpprc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yrknwsyk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wlbpzbpj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rylvrcoa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qbqeblpf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aianwhtd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xhmgspfv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kkytpqca.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbxaxpp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tigzotxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhzfisbw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3irjxivdk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kchybams.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oaspmcug.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wtwjmegt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mgkylzsc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xaprqoew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vmwuhvwt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ugyaywva.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ezhqpenq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwuwmesm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3khavudbr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jwovxdbq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kipkrtos.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jwtslpqf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yodxgjkp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3djjlcjvx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iuhuhegt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkujpwu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmudmmj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhqqerom.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3izfbiwpn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sawclexu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3idhsjsxi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jxsluzbm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jyfveiax.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bzqleofm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqclicsg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rulvoocc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jvhpcutr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wrhehehe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hlihiqkb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bwftxasx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uhaocpqk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsaauod.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tcycweuj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jgddkzly.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hbjjyksx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tsagpfch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3djldqdbd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3scoexbwc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqmdjgq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lwafkczf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dtyudfkr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ptabpuvu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hyscpjuf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pnurytay.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cxqttany.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ykmundcd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3raeqrmal.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mnfnzlqw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3okkcznuy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwrwddee.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nncwmsat.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpfllen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3miwfhcxu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hluutgfx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jlwjryuw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecztckso.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fmozfbub.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fjmofxki.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kjyiugpo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3imffngoo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3elvfqlkz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qhbuiveb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bvddgfhc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ahwqxama.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3asaemzkp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3htuyhmju.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3izkuwnbk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ygtuxvgl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mzmqjset.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idkqqgyp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtcefamc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpkudbxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3emgtkjmq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nphwahsb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lltthutg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ylodlyxf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xivponnd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rjffdwou.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sbguyglh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3awtsowuu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywmkgpja.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hcceufcc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sdekfdpi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3leunrkvy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dfztdygk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fymkxamj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qklidydq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrgkhkex.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pyiyftbr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wzldteqm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ejvvdttx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ojukgnwo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dlbqifhs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mexoeczd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yvpwgqrg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3szrrwhfs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxzlcqur.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsjqoxce.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ekwdgtwn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3htaeiakw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kdprrykr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqzhltal.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3edhbquvw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3awsyluek.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3inccsgnx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rdrcoxdc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sdaxopvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ubbgxzbo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cumbwsds.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uxnfwdeg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vpkzoqhl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yvrarxwo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dplvrndc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uschfpbl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rkptpwhq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3scmstxvv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mehvibrz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tlhyzxob.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ehprlhqi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aaumojzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjhkvgyb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uenohfkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrhonirw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3refkacil.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3suhwiemj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlfgmkfv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ptbvugnx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sudkgvaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqmrduoe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ikrtrslf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3healanwc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxdxacnq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ivyagqmj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3suvgwyqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lwyskdbo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rgnxwjge.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyyxpjap.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wlfpkyst.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jahpqhtp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eyptfahi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlufvsic.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iibdwjpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vnesvbgk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrnuhocf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zzcyqsga.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3upzvljgr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dxytzzxx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvoqmox.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lfanghug.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zzedokds.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gjayepsr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ybwwyhfl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qxpaealc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3onqwsxbn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aihnyxzq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dxkbqick.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wildiyyy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cwdkyqhg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hzjyjcyk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wnpmywks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yttoargt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vybbwvhk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aoplzdgw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmsysqhl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vmnnorxs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jexavxhy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enhwkrlh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvysjeyj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxuvbgik.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjdjxalu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzgpppnz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opzfswwt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksefdkir.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bnrwfxsd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3suaqxlyb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auycnvja.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ffqxfdmu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3meppkhjd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3branldeq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tccgvzmn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nlsalbvg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aquqtfju.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3asvughgo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vqsbzxfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iyplnlgc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fegshsoc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zvlhhybc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3odntghxs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsynzztj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmjhwre.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gsjpdtux.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rcvqxfby.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3whairxgv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cdejztjk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ibiaayuo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ljxnsfgt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3givchadz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkzjnwxf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lhxcfnbz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rynpvipo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xdliixrf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ldpratpu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flhmivoi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kfeitkmn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gttpwmzt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejgazubx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3psijweuu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtqutrj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzhfipol.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3oydfenee.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaviqlel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmehvlto.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mremktvl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3derttduo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtgdtavf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygvujvur.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvriilny.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fglowbmo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulgxjdab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rohjhlfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fysbcycu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pqmgmfuc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eupeyjld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xwxbciwf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mgmtvlsy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3camftfhs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qllgtvdt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ydzmmxsj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gmdjmqxh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kiuzejbh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zuhumoyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqgvjkol.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uypvhkoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxwcio.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3prilhlrp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3konxbomv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfjpfait.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iusbfava.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3novfwzmj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brebtpdm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zvdgxbeh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3otdanvki.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iuobrzfx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3epgxbkou.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3soxswfdr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjjkylgh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yunlkpyn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bzxqndfy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzldjevr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3krsyqata.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hfjqucho.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xwcwvukk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dbuhnfnq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lljxegsa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oawahpor.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3camyfcrz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xlhpbouj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3iqlxwpyy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kdzsrcho.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cjusfnbg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sekefkwh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qgfczrhw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hilwgjdi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ouvqcvwl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioglyfrv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpmdhbcq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfoteny.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3axsowrhr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3acmizgdj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3unsqhesf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cpuzlzvy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rvamqbzq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwclagpp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aybadsfq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwquxubp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnhuzckw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kcyzxijl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtnfrzpb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edfihkjh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gtaxbrpq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jbwtanva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbyjghes.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcwbvznq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mpgdsosf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwbkgghd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wdeovric.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aorszpxs.html


<!-- 参考信息 -->