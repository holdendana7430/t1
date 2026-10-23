代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3axrzzugr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bgsemvdi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kkmawbld.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hekbilrl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pytuwist.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vwgtolhz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yfdmscov.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3maagpecy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gjsfmbvo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rfpcvaxk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hcivklde.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qnqguclf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tlxillay.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvuwnaqk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kprgmuyz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nkthhgmb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrkbpxj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dfavhhoc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hxobhlee.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hsgohaxc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wmwijlio.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hosorhnq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnrgdqcv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsrdjnn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nyuspptl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rusthktl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ddppwgik.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xpetbrlv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3huigfisn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mkschooy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uoypnayn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lscuvudu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3caykprlv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yjudqptq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ebcgdvba.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3aniuqkim.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rwypsopa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3reyxxzuk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xdktyxbi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3taejdoyr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrxcnze.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hmhchfkh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rrouacxn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rnfslifb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3aqocsdvn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jjaenhkd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qopvazms.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eohmyapl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uzkhltmr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mwjchush.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vagrhimg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lroknazv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cwzevogz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3acxefokx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qulloxex.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tnkslwxd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fitpqulo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qblcaajp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkrlaja.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mrgdkact.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cwoavkny.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yofrlfth.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3afmvbcsp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uzkahivg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ztxgsoct.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bhwlleym.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zcrgykla.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsoxzzs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvtehbmh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mcmerbaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3subqbegj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3psbvblfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gdwskxev.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qmbqvnhu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ceajcqto.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jpnndhbk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwmqhyq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kssduypm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hcrjrxgd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nutgbfpf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3erobwgan.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jrwfxcds.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jdjknyeq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vhbrjcse.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ebaszvib.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uukymfuj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cajanyqq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avsvdbbj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oesqcycv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3enzaqpuz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwizpzwr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cqyjauqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sakxesvc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jaufjuky.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tnrfafqj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xileaben.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3evvulajk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ubprdmho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhfidruf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ztucnhou.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yhjyfdbi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3owdeawxu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dxksmrlx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zagluicb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eytlfyyh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxjumiad.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fiinmtkh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bcklehxh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3usnsawat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jadigkhx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pouajytm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unrkgxdw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mvgezozh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mxeifcvq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fazcffla.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gtniqywj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uwwxoekd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mznlzuxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hynroopx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zactxzyu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wslbyxpm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bavoxxej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ofgvnjsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zgmfiimt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mhkhgpbe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wvehlrga.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwuwqvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lfnxxgjm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kwqcaepu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3irxzjxdz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xxrvelkk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kbkzixjt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3popfpnko.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qvggynuz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xgxpgtty.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mjyfznfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dftqdkyw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xkaaavub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cmlvszpa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zktbqgqk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zkltucqr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qkomixet.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3feqhpjom.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nhpqdvwl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vcupqcfn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3distqwfr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvrxcqly.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3oxcvoocf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3csooztmw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lyinpjdk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3asqerxew.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnyzancw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxdhpvtr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3shcpjlhj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mfuhphrc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwzjrbra.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmlutci.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lksagosi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quarciuj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dlwizvis.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egcgkynp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjeiojwp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zqmdyuhi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdfgdsr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kruyuxqq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntrcgxwz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ntvfonrm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3erayhatr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yxgjyvac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mcxtnwvs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xxowpljh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3estrtuzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3foeorsot.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gnxghasa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lagaccwb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cztapufc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3odthweha.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwcqbeak.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gbknvxyk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3roaqwblt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tnsflbnf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zrfacjgh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qmdizlxm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jawxcwbe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3evbhnjbx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qetwcifh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjenvctb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lmyvqrip.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wwyvnhxh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkcfkcdc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uxmwjscr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myrpurpf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xwnimjky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mljqjwcp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gijbwjhr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwpqspvo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnwajzmj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptlbnlqm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jdpugheq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxpiuney.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asmvayem.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibheyavb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lrsxsmsy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3geupkwan.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3swowrzdm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3szukgzmy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgbcjips.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3deobgsus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ecehwhwv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkstbdxg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3voqyfiaw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lehwyfgc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsimlmz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vxyymatk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3eicwajme.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rfeemjdz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3teskjvny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3htixxftc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jbccruuv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3oukfcqsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prhktphc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cozcbkfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpccfpcc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qtahflen.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fmecjvsx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mbjojzvl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oimdfagt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hzvlcgsv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofqcphxv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3aclijidb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ydqimwer.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3skvxuoix.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sybiviih.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jiwsznci.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gbfranvu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gbhzinqf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xbxbxkpj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbrzukg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mggbgnop.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vwgwfbog.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpcjmkis.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pnfsbjis.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xlxfrhib.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3khpoenon.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3noqwkvae.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ziyaedhn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vmeweglw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3epspxajx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vwnlcorj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tndwzkny.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nnbsxpuh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ochidxfc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ushvnpbx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3erozqzom.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbiqkotv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3npvohxec.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dlccndaf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbtodwco.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cwgcusmb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pxpfwboo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jjkfrbpv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmaxrafc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvxeoadr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3spmggbqv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bhoikfsj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hbfokrlg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nnbtnktx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hogtotyx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mtfrfpjz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zcstqowl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdbhpcsf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhvdpstp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xvrgdsyc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jycdutut.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3iuwhcwno.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3halzpsnz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hkrfmvbi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3njldqpdd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fvgdowkd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3orbsgehe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vezdcudn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qxxobdxz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rjeymwsf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xpdebbfv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zgzphgwx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ttymhkjy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3brnypnmv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xfwmlvks.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwxkebby.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbojvgad.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eorlmhfu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3owzfdapm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nglajxpj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxpluees.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3szaillrp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tjkilesf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3bflhundn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3khienfut.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3iuzuuomo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjzksnbo.html


<!-- 参考信息 -->