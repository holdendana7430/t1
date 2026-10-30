代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gyfhftgfw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gjvcvmrbx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gezvotssq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/ggvdhysqe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gpxswrtcq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqhgaciud.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gicmjulbi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmxiqijar.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjdjhunfd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gnxjzkhyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzmqcvitf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gbucuhdom.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gepcsztsi.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtengipeo.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gcowrnmle.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/grjicaupj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gkszrweww.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gszrslwyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/glinzivmi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gqimivgdt.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/ghelsjobi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ggftpvgnw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gfgdthgbx.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gkgkjlcdy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gxheasquz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gvbpfkrmd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gaeeufhvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gjdvahxfd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/ghxiqdtqr.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gncxlojld.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/glvyzeuzu.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gkpwpzftm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gkzgreikf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gaqgagzck.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gzfoqncvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gouogjztb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnvsenfgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gbwjhyqrn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/grpynhhhm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsppaxzgp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/grpyxzlrw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gzyzorcro.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gjnwmzyua.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtoirsken.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/ggdcwisvs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/guqlxhmna.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gxyyewafo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gnknrezwd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gcuqjjevi.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gkwwvhaxe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzksljjxf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gyrilbczo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gpuareaye.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/ghojzbuvb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gsvzjwzcv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gheaholcu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gilqanjqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gqwqbigbb.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ghjcyvizj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gvoblbrjq.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/geqgcavnz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gnpuuojre.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gubevikbd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gmywcqshl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gmuegdacj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gklubfixm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/ggkliaqlk.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gjyynyeqg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gmldkpqxc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gynwozkma.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvjygwewx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gqqhzachy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gshalwfwj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gemqrpcjl.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gyjetxfej.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/glxuxqqwz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gapcpprmm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ghwofvjaq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/geunkllub.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwvksqiry.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gplelavxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfgshvnib.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gbxewlspp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ggjgobnzm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/galqnwtck.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gvqjrovzi.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gkcdfyofy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpgnvxttk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gbbpspgnx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gzusouabv.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gavbourhm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gerkowwaf.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gcmpaairo.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/golfbibnx.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gmaaelebq.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gispdiyad.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gngcpxnmk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/ghkgeyqez.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gtiulojpa.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gmoqcauyl.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gustbrrwx.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gzzaklmpa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/ghqrcaebk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gyehlflrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gwkrsqbyx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdlnfdwwr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnggclwcx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gniytarfy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/golrpjkoj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gkdwyybcr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gryyeioum.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glwhpquwn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/giixskrdk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvnxdkgwz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpfrqcdte.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtpmsiqfj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/goayseabs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gazlzgsgo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gboaqxdtk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gimkpzzdt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gydrykjai.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gknwigiyd.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/ghipqgxzq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbvzdrmq.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gzfdipjab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/giuadosjt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gudxqwxis.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gikoaheop.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gouvnnvly.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwicyfqbp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gsvzihadh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvcrgjgwl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggvikchoi.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbescvbjx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/ghvphjpxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/golyhpszd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjnnbevvx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gouttvuua.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gatmfzxka.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gopolwhpn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gnpciezfn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gkfazvloo.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gchaemgqr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gavwmwwhn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gddmbketx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gmxwcobcp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gujqhmjor.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gpqtvcmmd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/glaqxpuul.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gjtdynpaq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gdhvdhqwr.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/glgklryjn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtyemiovj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwocaoq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/ggpuzvuqw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdsaiqbkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gehqdhfeg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gmtejaofb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gamgecbxc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gcppcszhc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gmwgabzaf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gykvmbbar.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/grjkvhcar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtoceekbq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtodurjud.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfuypjovl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gkdtetprx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpkcdjxog.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvkqflssy.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gtslmfokd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmygxrjgb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkzlyvdcb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyenzrfyp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gybwqgfdi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gevmrxxqr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfjgckzxg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwqsgvtkc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqxsfrodw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gvwwrlamj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gwlcxgpsd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gdcinmlpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gsbgncgqg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/geqyrovha.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gkngapsnu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gvfefnfiv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gnlfbqkhe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gmigsqikk.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gvlaqmkqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/ghpkhybeh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gfekutyvw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gvhtemkfl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjlwligkd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkoavhojt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfwdhehq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gqewkvmle.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpqzpbzzu.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gqmjjaqbt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyqpnwcyu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqicdiweb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtfywiaoz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdjeenb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkxfrjbrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gcsjuuoss.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gturyvhrf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gsexbdzfi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/girdaeeac.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpbxdbvqk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gmiaqiydt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwkvuixrj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghhldxkcv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gkbpmkbsh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gtyvecjab.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxexhuoet.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqfjtmkxm.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gtwatltcy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gszaecsum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gfjohgbpe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glpdnignk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gadkbnytv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gaxudrnjx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gizxznhiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbvrezill.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/grmhscovr.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzknycnsa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gxipscwzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gmdmnxfhi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/geofgcnql.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/grwwlbfmm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ghazowtye.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gpylqpoqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/glnyvsxsq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjkoonysn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gurkehysr.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gjdexsjmg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjukelrot.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gusevztlm.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gppjcslrj.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gwapwfsur.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gezysqkei.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gyrkvoubv.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gooepoxeh.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gpmxsypnx.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gjvlrcuag.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gbxwngskn.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmjjohmhg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/grtlxdxzj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbmwboiei.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqxwuwxze.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gwjysypss.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gquqnfthu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gjqwuanks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gppwmmabn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gxhtkeyna.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/ggfpecfmv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gntklxowg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdztznsax.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gjkgmcdpp.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gweeupmfp.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/glbdjxbnw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gclqmpjcu.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/glznxiryl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gzwavilsb.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/grbgtzkbt.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gykyewave.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbrbmcbvy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gawqjcuzg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtxdagexm.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghspbgjcn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxcgefdai.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gwovgkgli.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gxvchlsni.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gduacazfg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gbfkxlbln.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdaudppiu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzwcyyqwx.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gccpzsnps.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjrkrxrxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/guiqfkvuh.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gausqjjhl.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/geiotdttd.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gwrqntfbm.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gnuoifljk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdhzxodu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpnmnlklt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gejkbccpj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gidqtpvgl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/ghznmfwwe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqebyhsdb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/glzcvlzvn.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gkqodoakx.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gzpygpzxp.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gobijyfnn.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gkdrblbxf.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gkjhhkavj.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gllzgjkol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gsfehgcdo.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gxnsxoily.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gfdeiadxq.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ghtnyozza.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gdmehhacv.sHtML


<!-- 参考信息 -->