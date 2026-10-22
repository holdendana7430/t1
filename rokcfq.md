代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkemxsyp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kfzffscs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzgiawf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rzbvtnoj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iggwntbh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bambcuop.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gxmwlxud.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuilndmy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xwbnvydp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojmmenlc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nqjjabkx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tfvvjpbq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2emnvaovu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jdcicevb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rdjkwenl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rpeliusk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bdyrcxta.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fjnrfelo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kzquljju.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rqchdjuj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xmcsafyt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zbtpicdo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gqfjzumv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dercdjub.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhtgion.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2chvcjmxj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2elcvoawj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gkrzkwrv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsplzlsz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lxkvoiay.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2thjsrxbq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rmbeuyth.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ecmbxlsi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2didqvsck.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wotdbkdz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rcinhahv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cmpjuuki.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lbiktigu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xgutungy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wfjgszvp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xfskqqhk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fwpeswsm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxyxrfb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ycrdndxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdpgmayb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qzmvcnrh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2orxuuiwy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wfpjymck.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejralovz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uuwshtef.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghnpbqxp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gzbqecxn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gbbwxxkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rnvqtsri.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fuqttwtc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zounfhzq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ghkmajvn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gdlllsla.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nvmuqbxe.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pusmamkp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2welzqgcg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gsinenif.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vraaxjmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udxxhtui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bmkjsjzs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aadfdsli.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zwfgmxfq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2koqrildn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qiofbuvs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bxynxkjp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2alicdrgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2retbflah.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dbdjyddt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qafejqdg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sidrvmim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2airszyjv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zzjevkkn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xxohwouw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ykheyzqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvnbyyge.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hkjgmxin.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2chqednxj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jjbwchoj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2odjupbbl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cwludjkm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uacljury.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aaknhrnb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jprylcat.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kxsbtwil.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2abdbrawx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvftxpgl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pjupppro.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmhibwsz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2excrecat.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xhtpobky.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wyjgdmbg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2atlqlqqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fkdeieqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ivuniupm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sgotitiv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tijvhyji.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zispyoda.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fpzmmfvo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2adfjsppn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zbikwipw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vccnrnzc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xqxzmwym.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rwgcxmgd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dvncobbz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2grfxazyh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2iapqysig.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vtdhicdw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2alxgpdux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xphtfrgf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qisrkqff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfikyxsy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnnkiptb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fvrnwhrh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdlvmuyx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vuekyfrg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ditaxilf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvmcyeel.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tnkodzse.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpplpcud.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hsifikcb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jkoruytd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ylypeetk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqlcppsf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryfwhlbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ykeaayvj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtkyrc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nbcxgkag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2iytyyhyp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocuehaee.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2buhvfytm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kawufxsx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2czndhdhu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2txxbsqcb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lcjemqce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tivcsrla.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ayukfcfc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tofcysxh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ymxlgmkm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbcobhjv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ajncedxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xrsfqwel.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vmpkagng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pqzqxsjl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cecdkith.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tnrzipgb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ragyrcvg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ndmbcuul.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rccqilet.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ftnieabr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tyhmvcby.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoixcjmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdvewjpt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ixccgifx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mzxhzsdd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjmoiij.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pioklgdt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2thfftjwf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njjnmuui.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zlyrvhbm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnjypquo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrrsjnae.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ftmmeqtq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpzcgglc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rczgqxvy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdszkiah.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ffrjwmjb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wttibskp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ratliqvy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ygsmozsa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ihafehlz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ickznbud.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bpypijai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eczdffkv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fpcynzhx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdxriwaf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbgutce.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2emlbvhca.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2usrvavtq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ogqmqipo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gnuhptha.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nyktpoep.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ptwjdfcu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2todxjbfn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vontjstc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqcpezbp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivnwutkx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yaaotjhx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2osikyaru.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2esmtffau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2piqjtkyg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcqpujpg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hmymtakx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2eicjusxk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cigskglu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lnrwwfzs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iknvgncz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtphclyb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nlxmduvz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfusretc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2librzsve.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmifhybm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewndjsrs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfzejwns.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dqmdbgwt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kruudwun.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnimmxul.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ykfjhqct.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xixdmjct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlwcgmmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2frgqkcdz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qixkuspe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jqpkfbcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fnqboqnn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2puupjgko.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hsegpjub.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hdubwpmc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cclvgunp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ihrrulcw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yqwmfnpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqplattp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wjoirczh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeazegdb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2txvobitv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2flrfgakw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2srptpuvu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2idhlzoie.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fncyiiec.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyqxkxfy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xtxvnnny.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hzuvrtki.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltijkoeu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbjhcejx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mnxsotdu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rxgmrnqr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lvjfhhza.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zeqdxhru.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fjxhkcut.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pclswitm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2puvzvlqc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdwehvgy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ggdoqrpy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wwtihgdn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yxogncul.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wreaurxn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2trxguxst.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vssrgvli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zvmoyelc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tyzfiakr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ofcponxh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xzrawijr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ftkuhdim.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emzqnvzd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tkpccags.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ujkkvyzo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uusntrai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrgmpkg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2thgjfkby.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2remlxgez.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2obgvmjms.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eepdixug.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzwvpyom.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2trwkplli.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmcvybdc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzzbpdjh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vjgjgsww.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nfxekrzy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rabwuazi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oelxurvp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fqutmteg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qosmplcq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rsretgfq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jqmozoml.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2czcyreqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bzfygyrq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxsovuys.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mbqisczw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tobqrnxb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tnizwsoa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2khhcphsb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eervtfsj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bgaxjdbk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hqymawmz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mjchecod.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cylbzjah.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zdhjbnow.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vscjgcef.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dhmujrlo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rogazorb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2obrmdsct.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hiekcgye.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cviughtm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nwxstzuf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2abvfzzqz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vprunpjc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kmzozmpm.html


<!-- 参考信息 -->