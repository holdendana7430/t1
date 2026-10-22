代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2omkphnem.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2caqwzqvn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ivldzvnk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2elgzuwvr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ngjtmofl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avymzyyi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tpguphqq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rxtpluic.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qowyqngw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlujbwno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvrcbih.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fndkqtvf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zexelpsw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fokpibeg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2uvqdeeyf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hjejmsko.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2exnniofr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qnzoxhig.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsdfkfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hgctkisn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bjtcuomj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ligtpbbu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ferzcvha.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ikrfbwxl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrxyyqye.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kpgtcnzf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vtgnmwyc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2djpkxlau.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fzhyafuj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2twceilwz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hwbvncdc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yllsjrnx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vqdebhpy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wryttazw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2droypvoy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2afsvolpo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jdovnmnz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pnyavkvr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2uztsliwb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2exwtdgut.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vbbwsybo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikyjqsrm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2udhjlklb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkzksflv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwxzlld.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uniwvgfl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2avqoajan.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qorfgajg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2afctkmuf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ftkelqcm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtfjiakl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmbxpsz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyekhnn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2atbjteak.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zgeiaxwe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzvmtrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zzkrkvsr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2diyoiyrm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fccnztww.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2phbaxdkl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgnxpecw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2igzrpeqg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bllloxkc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfwdrqwv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivcukfid.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dzncppum.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2voajsrbb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rawhyeap.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jldfoaog.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rhcobxpp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2loutyerl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2euivpvon.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uwpjfahi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jcgvnvjo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhteeos.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hwtxcsmw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qxphfssk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cgzeotvy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vilsihps.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnyxugj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2iabrvdaq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wdeyiazc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrrany.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2quzoazdf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ssbdptbi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2awgcipta.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qsfqsisc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2axasfwwr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cflybrah.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pemovbnl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrdougw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zxnahwft.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uucptkrv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nxrjkyqp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ovlyqfqo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mekryfhi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qfohsgmi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ucpnivun.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2etarpfby.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qcvuhvfa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2agadpypp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tpgftwtj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nkbajhoi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2etzsdnyt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pzcioftr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hdvdqxmz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukhnhdpc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhcauxve.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2asqwwmpe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mabwumgn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gsxvvdhe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bldazhmf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2snphtcvh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oyggjxpy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vsbsuwgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mpsvkfli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hlmbotet.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2klxexzbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eeeshxzq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rvnqoomw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2knnkrkhq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uihnbfev.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oxdmeozq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzvyqqsw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zxwdjahn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xyjxltjc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2eurqdavy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ytxwhuun.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cgvufcll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixdsgivz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wqnzdlzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlsmeepk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytskxzha.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2snxsaqvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2acxvdnap.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hahybxxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jbkkcovz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pdbujbsv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ugxshlkp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbcvdpbi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ipmhptja.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vadjlvmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mjqtajlh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wbcgmnkr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ojgcicvv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zacswboo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oymelkkd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eiimmsqo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xdlbcmpf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dgknmojt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2emcrozez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2amnlhqgz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vjqxqtxs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fgkdspdz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lrsuiini.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pmyiybpv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ibphjthv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bzexqytr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oauozuyr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfhcbviy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gfnilgse.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjksjbr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2avcvxjyo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fmwexxft.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bpdflzwj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mvzmyojf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2awvxdluo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ejhskuen.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bprmnrmq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gdnfcfly.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdexllxr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnzbqfxs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbdnmtsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jeftpudv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sheeeqmy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zewqkbun.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cctmdhvk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uiqcaudc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptyoojyu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hgkogaem.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aipsfsze.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzzourm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ousiumde.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgsfzpxb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqzoedml.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qistxvfq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2uragajde.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnsfyqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eknagwzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vavdvlmq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yqfefodz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iubsoqvf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yjgnubzv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mvxtqncz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vmkwhcib.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rdbknuys.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cugvatnx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vmpkfjmi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mnzohhrq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ifjobdae.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2euavwgyx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zexyeejs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2otmroobw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ezqvdfbr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pvtwrowi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfonsxpx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hjpixcur.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ajoqgenv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wnvovvxl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fqxfxeym.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mfngygfu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbkpnmkv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2icjxklog.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kngfulfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwfclrzr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooeuulqy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbuluglz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmocioyk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bvejjfqx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvfxnplg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iljxdgtk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvqkgjnd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ymwsgsha.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjnomzfz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vilrgxni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfncuqty.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfhzjpav.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvlwfcy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fufovfgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxhtkjah.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rrpuujcs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yqctyzcl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rcpmxyah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2toqesygu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bszseakx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uzbcfocc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nexofraa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jgtozkcx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dakqtfrh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqoexp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iesoismk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lllhasha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qquualih.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zpjhgusm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mchndxia.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rtuuzkxj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ypgeugaq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyvwmnjk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ucemwaes.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yvutsete.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwbdfuwf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2foeujrwa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yirsolso.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2lxpkajoa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvbmsnmv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwanneje.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdxjfhew.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ymovmmbn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ajhlxpwj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zbglorjf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tphcxnmc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vjxcufzl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vkuwwpum.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2trfnypvr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nueuzcbu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zjjcahqd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2leufoohq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kcpjeoog.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwyxvc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uqmpzfvr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rthmdxib.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xqanbxtu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yehdtgpj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhzjvqtl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adzhtyhk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbigwoql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bcakkkoa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2omiaxhdf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jjeiupun.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wequpmcq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mkumpvaq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtooll.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jqouhhjx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2afvfimgi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwttsaeu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2iapeitgo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxwdrqsz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ayccuaqq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hrleqyxl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kvydihdr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aiscldys.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hardjvjk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prrhchsn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2esjwjbca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zmusbicj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lkxweuzy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gsazrkva.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2caubvrap.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ezqzbtsi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mfutrmop.html


<!-- 参考信息 -->