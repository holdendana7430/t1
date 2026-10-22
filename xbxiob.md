代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2scppvvwt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zixejtus.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2frkmifgd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xpthdyei.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnkiiajg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bybvgzkv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hjyfagko.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eqmjmwoi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ucutacza.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lzahffny.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hqnkhejp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2duocmlww.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zwjktxdw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lwfddsjt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jbgazpah.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wlahyehw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrdjlfcl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vvchtkqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xypvzayi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfzsuxb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2femyiuzx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2aiqaifay.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fplvnhii.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajscktgh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2havzeidg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lmnzymgg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qoeouaqn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ijkvqett.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cictzzdq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kxghlcom.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qyjnwyjn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uypqnusx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bsvuvdjn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2byvjcxaq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2spajfcdm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xkxkdfpo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hhejouvx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkaxwowf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2yqwxwbzc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gpdscank.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zypwwiyz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ybbfjgru.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ntonrcsq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcovjetx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yoijwlaf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wnvytcih.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ubagchwh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2psblvmrl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yvbahykl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xsdavuli.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oytimgwi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qjapyvrp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbwpupu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eotgehxs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wppiexkn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fsddfeww.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gpbsdrgg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ipbntpos.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2umsztjpi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wpkhawgo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mvshitqs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gubjrdcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvvtmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jpvabdal.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rscirrdx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omiieumh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ttcrpzcg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrimtfjz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xhghyuww.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2teshhznc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ruegbmuo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ijchkhaf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dsuxyfed.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sxogwlox.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mpkgwohe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lasqamwn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pjivetok.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sulcjqyo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2khzjnijb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hbadwwvh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkgauwm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bnkqaxkm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mpqfufjs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yavxewos.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2djzmnkvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sffqwwdq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gkcgmjyi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qlejuwnq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrnllvn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kqjlrnjs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwffgok.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mthlpmoj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bnxnnzkx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2azimmked.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yzhsnjfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bubhdyuj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rrxiqeid.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2txskaujk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xrwjobrw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tkijewbh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zhhaopvm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oyqnolpi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2myodlalz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2neqzjoot.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rwsgynvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdowhzxu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bnfpuenw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vawfbbpk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eoamphfd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cwsnfqzm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yydylmef.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vagwjkfk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2klygyrmu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jrrsrkes.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xnceevhj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nitkpczi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2twkjiako.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2reoqepuw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ssnxtujo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2llmisleb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qwzmagiu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jbbsdlpl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ohziofxd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rcwjgoaq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2glzraljc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oopsmklh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2adbfbzcq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uidbbblk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dtcrcxkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kntbjgkx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wezcghdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpgxchdp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tvuftfnd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jugjjrho.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lunybkyt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xiroesoo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pyrmuhag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2glvisahb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2niuhmaza.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2msnbqcth.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvbokglc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqxoklpq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dkrheegf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnmakdb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sktogqwj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sjemskwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yybldbwz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yahpsoyw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2knwkpzef.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dvafnkqa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2brgpumam.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hevihpmt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ncpnfnfn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dabuvoex.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ciifabzc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2udiixlmv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jinajxsd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xllhekhj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ldujuxpd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2edvacthk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jaymwhzi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qlawgvkz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gnpnhhuo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2txybfyit.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gccfwsuo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2czcmeqwo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytcochzp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yljygplh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2webrjsyy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tsoxmuyz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nmaglamk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoguxgfg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqarkxks.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxfigpeo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yohhvlbo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyhniskm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2duexbkfx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uhgnzpea.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuawunqg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfehldgv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fktpihpw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttthodut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cqqestmi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjlgcanu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcsaokmb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ouxwzfyd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2myssnzdk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qjsrizmk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wqzttpyl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mxofyitq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tennjzsl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2temcyrtf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kssexobl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zyamnunp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fhvlkajw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ehiotari.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjwyuke.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzhucvzn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pasttfvo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ojhgiyif.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dnwiscsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mgolawtx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2udzuuxut.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jrofpyhh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ftagjrhh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scytggae.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qiuxxoxu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ilmzbfhn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lyzxbucv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yttbhspn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2znbifvht.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lppcolfk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mctgevnq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mowoqkgl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuqpjhgo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mbnljjes.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfjgnmr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smgfbfhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ypqjryjm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awapystm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlbhjnbi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwcrcri.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2inutnqcb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrlaqgts.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jupwjtcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icvrhzrj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojgobxpp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bdszmsmz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2taokuwzx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uswdnkae.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vmhjjxsw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yhkaqotc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqdigif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2azisnwix.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fookpwap.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qzlcrkct.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bibiyzfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rjotpgnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rtthuoon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eamumsuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjrremtx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qblxutqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsoiqsux.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jtgccvyw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xsmflgaj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmkkamgw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wsilljan.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfodxnwp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nqqqjqeg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zretadca.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hhfpsdkl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjuyuatw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nclkoxdz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uiwfyvus.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvunogst.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jpgbovbr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwskgyoe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mpdrqvfc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jqunxinr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rczivsam.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnclkvlh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hytbojjb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vvswdtxh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rbdyzlpw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mqhlupws.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nrixnngf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jtdzqvsn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ophvyfso.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ksonfude.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tbszsujd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wmbmekuh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gbcttbhi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wijcdncl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igykmxmc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qcbmmqsg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2docmlmwt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tzvrdztv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqdukbcn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sytyoecl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ozdxcugo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ugdoitlo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kbxmydiz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2znuouinh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbgsofqz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2skiiwknf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2utqmwupo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2iwddjuen.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rzwrjzjx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jlyfthld.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2havtwsvx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blwsejwl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pgqqfzbt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gowchstx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxuhypb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sbbgahze.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgsntzzd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hoaoedup.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bsyauadl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tncxdfsk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kobysekd.html


<!-- 参考信息 -->