代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kzpoucew.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mqseqqlc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kpscwdek.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nrubrfrv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jidimoli.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kzxasgeh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mkjnwmfo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fujlkbvl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ttxulmpp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wzkspkri.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxnkzols.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xjyngknh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lxhciapd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nnmmzsgr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lployydb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2heztdaga.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2umrqxpsy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2drcfhste.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2sntydgsb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2thpcekxw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2icvhzvfz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyexonl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zputajwk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cdipfiyy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2aemwbmtb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cnppquby.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2buwjytse.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2duxgdcnt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhpnezmq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcimwchz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kufnimzm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ydaryjil.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xkgwwems.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ioybllpq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wackarct.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2juwzstub.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wqeknfhb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pgxowela.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2otduoupo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pgilzvgs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nzyjfsxh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fnwemvhn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mybyjkuc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lidypnkg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2okilscng.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2diycoopa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdpdfroy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcrnlmxj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pziayajb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2seplaqhm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ixrmhvvo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbiazvz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nxyaalgh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hzxmftxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vqtgfkgb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2koqtjmfv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uukcchcs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dsnldsac.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2folzpgyz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2daktdzby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xgpndydq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2osvcvwah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bjxwploi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eoilmayr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbspguoa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfzeppjm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nqxyizkh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlriepl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2heizngcy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uiivszkz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2blwrrvkb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmsrzqaj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rwgyaotm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ieiwchbt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rwyuhdpo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eivhlsak.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kzuhxidx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rspwlwjr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yrqpzukx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fhmquqdb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fnbmntay.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fblrndcb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dygczdyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2syomriid.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lrlaijpf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pcptimrz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2luwloold.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nwmwxkpi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bpqclpcu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ilfqhwhn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nicfjcwu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjliblw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rztadkgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qkbqnpqz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iahggpox.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2elgklsbb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ximcklqq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2abvpbpcr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2smryslsn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhcebhhw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nokusvcv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwaawwx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfmausxx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2uipdduvm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2szdmicea.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2drovhizj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jcwefqof.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ajnzxfcr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mxpybiwe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2guqxprgh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qpvqzawx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2asjjxpfn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2boaqzjqt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qevgyazy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcntqprx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vcibuydn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jckakfzc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qplhsozs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2duffnvdy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zgojnvzh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mzjmswmg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hunbkygk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wsabrwjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zxlgrlrf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tjrvzblx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kyadrjpv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cdgjsdsr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fifrgmjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgsskbtk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2myvalhwe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zzrfziyu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrheaihh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bulewsdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvvrbdzd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xvnznqng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2godassno.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hspzzcei.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ngukwkkn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2moyzwykm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jeiwzpnt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iaoiomru.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xeuvdwkx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uvyqdgrw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uofcesqp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mxdxbehm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ggfamtzp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2phpvjaih.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xlfnkhau.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgyybnim.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpugnyjk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2quxkwxyf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2atyipuus.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ianichwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wbtmbont.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bentqubv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wjonmrsg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hhtvhtti.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gzwgjxvx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vdzovfrc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bdfxsxxl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wqfldepv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2yhfjkhla.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ydoqullv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmblivwe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yrtedfhn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xwapnguk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2daskzsiz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wkhlikvh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ryjilivv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ulkdrzbj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2icfrzgea.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wgqmcitv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nimhwccs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yoxhqtsh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lotartpx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2advresch.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpsgclz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mpapwzlc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rgodatxa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evaykhsd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vewkzwgy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mmwbpelx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnuknpxl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npefdyhm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wexlgkaq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbbeckte.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2caboaenf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovwxtain.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqqogafs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2djbrkkvc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lxesagqt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sjnxmlwv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xsbylpdj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pxvwagmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gpilmfks.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2brycfddg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oasqwoyt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lprswxtm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lfjzapbl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pofuxgiu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2spzrfqed.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vphjtqvq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2znunxbbd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kywdoztp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fiydkmqx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wcdprfik.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fogmswyp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfzmnykp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ybdzrtoe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdogrhbd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qswqzlgi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kbixpctj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2llzlbznz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqycjsmv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gmfbzcwn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqxedxbw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zqlixkns.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kivdwvli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgkmzpgh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhcavkix.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xuqpxzdl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcmhyywk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lzdkraab.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erudpqxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbtwvvqs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqhgouhh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2asajzsag.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gziskdqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwjordvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmnjkvmb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ougkisck.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hutxggig.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bktctsgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drkglaag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rubmivsr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qntzonnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2saxhtgnx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2naxumoru.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ffqsnqcm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xhmtdvuk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wssvicba.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hvbchily.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nycodcxi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pzvjohxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vurokoue.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2erxaajvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrvedlqv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2daeiwgph.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mjjjdaly.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yxxnzhql.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ntacamym.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqvozpws.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zxsjemmx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dadpubeq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2azjoglvw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yvyqcgko.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xupemxnn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2thjlwuek.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gxlrjzvr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmenuxyb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qxexfchv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdpetig.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zlcsxsfl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xsxagtev.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ixuuppnu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aqcibtqd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2goypxmxe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ykggcekj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vclvgpvg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2osiumcxo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eoiauxxp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pvramvug.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nhnuncdk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hjggwzry.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nhayyjab.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lyekcrmz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zehvprym.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2belroxyz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ommiydgc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aukizhtz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kitrhhqu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fmiifjbe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2azpvrqnv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oaqpdqfo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2migplqox.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogasbaht.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zeapicvf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gsvvyxgo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bagztfar.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uhoognfk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cytragkq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cemgpimr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2htdvoogh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2owxsyrii.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhgqjput.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2stzsoakb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wvuzcaos.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcobyets.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yxsiamts.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zhqgemsg.html


<!-- 参考信息 -->