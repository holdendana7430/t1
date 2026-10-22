代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cvljkfzn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pmgevuve.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2aasdjxnc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fpngsjlc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dedpiwxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2svghgjbp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqmsuyw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2svgzinto.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wduahrlt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tofprjaw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgpwqfzr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2anhpkivv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xauaorvz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eqmaxnwk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2payxfztq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjzaibwi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzgoszt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aktlbmxm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eesorirp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mmytnbvv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nggyoyvx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjkaocli.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ariwpkmc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbutadg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2omigngiw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fwrszzor.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qukbpogp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tzjlpngg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pvzlsfak.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2omarotaa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jemporac.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fjsdyfmc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bdxfbhnp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtaixpei.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cuaavtoo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vqiitbzn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2sehcgsgm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eatgjxci.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bswtpiwj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2eamlzilt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mozgfohh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fitklfnt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hsywknji.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvsoxnf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2txgwxrtt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rwqtxupi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qjvbqial.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vdrfzryt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hlreggmj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kufeeczx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wguyabyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dzpsysme.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdfulhu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mkrdnbbl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pdtfjsjt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yhomfina.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2etfxthxj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hjtrqhgm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvftnyqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lylgifbg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ykwaxpzw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nqsmyewd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wgtylvqv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vchsrlhm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mldzqkda.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdlirtx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bccdhezt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cywwdspc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxcjlon.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kobhgylt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zsbfqqfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zytjajxd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rpzlabnk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fthyshky.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kwevvmzi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2brygxhpj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cuhugcaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2icvhiuro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bizmgcmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sqpseyvu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbkokph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dyzplkco.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hnnrlzbs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jeefijky.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fzdxypww.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gyqctxqi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rqqqalqz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2anwgpbvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ueqfcrfn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ntdowixj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tpclzpcl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2whprxaut.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dscbhujj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mufnrkcj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hvmwoqvc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsuqfbeu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nacxqgvz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tfznknhf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zelppffi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qhlmrkhu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ivnlswap.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nekqssdo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qjowxiqz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mbgkbace.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2anxgpxhm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xbjzdbyi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfordygd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2khcduzad.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxrxdxum.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dhpjlddf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udrywoge.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zewyxnes.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jpyuhcvf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ttvpemom.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzdpsmic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vlawtmew.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mmffkxyb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rggpejvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yusnkevf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pffrexjw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bxyedafa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlyeylns.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lrmejwes.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uvrucxak.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vdlygydc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kkdswbbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mgitrhte.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xfpshjqm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qvitrzbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnlhfttq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ruvhmpvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeebhbis.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ebyllruj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2stbeupfx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdbzttpq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vmkvrhfw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iskcjfuw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hbbfqxrm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dzmtxebz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmdsmarr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcwiudmm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpjmhmik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ubrggyci.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2frfajbxk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jbfehcjd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2odwhtchh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hrucyspi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lybqrire.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pawqyktk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2arghoswx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2adtfxvcf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2adnlovfj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ohacsdfb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2btmjnjsj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tuqqtdwy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bbbxosuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2efuwyhin.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rapnhbpq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2emdehqyj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tioqkabt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wgcifite.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bpjhabfc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bnwzgbia.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ppbdzwlv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yopokyfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqngxwf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xioeqlkv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zgvxuhtt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxrzbpla.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2anletcfr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvvvczil.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zekfoopf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfcnqrh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgipxjuo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2flbbsoxn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsjayhis.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdzsfqrw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyjfszob.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhixwnbs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cukmnmfz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twvblikc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhjpcdtt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fnfwzyjy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfanfvvu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upvzsybw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wovzdacq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yhlepukl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrjileh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dzmazbky.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2liwakqoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ekuxvexs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2peunwvgd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sovuyccp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hmwgpajb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdappj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pzlyuujz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kmmkugxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2smppnvps.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qsuejpzf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mbjmunda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zntigaom.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hnjkzpoo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ouxiawnz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mtzrarqh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2quynxcio.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umwczyqy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csdctoeu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nrqxbiba.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bhjtkkrl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2egogdsoq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2alionzgm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwxlnlud.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ebnetofs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dhcdgcxv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxyeozfe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uzbwvwjw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2raunoyzp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2anvrwfpw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2maolreeq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eteriwfm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeauzqmk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pntdfjzf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zzhbxwav.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmibnwxo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yrrzidyw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdkgwocw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dawgowds.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrklcfmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cdiqzcrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxbgrajs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2swuyriwv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rfgxsczq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vfvwfkmk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hyvbiojr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hfofzbhv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2elftowtk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ofbjnuuv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zmxfqmfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2orggivdc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ezefamcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgehylbd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2stqemrzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmdfzuqg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wxnbsgup.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yaigphsx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdfvccqb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yobjmaly.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pqvqfdep.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2diymttjp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wprkpuza.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2skmvrqqx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifkuwvgr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yljjoidz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nmuywszl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugpwaqma.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yhemzhsw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hacytswq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gmpsierh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qxgsockc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ifndqari.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymkfvopc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xxpztivu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tzksyfbw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2usigqoun.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aehljiez.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ratlabgm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ahezybii.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2whhhqalm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wlohsuyk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hvcjjjau.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uuuwlenl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xkpsxrvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2afthwqfj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxcehdtq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ujgkwblu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vslpvqdt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ubiloyrq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2okreqjbd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yopcaujz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2amylfqiu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ozelpvzc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ddcmcoxd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mvufetvs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2loqxcyiv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hramzyhv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2aalxofxp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtxlkxfz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozroeung.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2noxichjc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fntjmgtf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxdjhxb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2utffgrsz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdabewhu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jsmbliny.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hjdhxqpe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkypilxt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xejqdmdu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xqgkzeew.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2emrkhrhz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ijkvbmbz.html


<!-- 参考信息 -->