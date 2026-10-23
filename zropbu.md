代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gvgpfkuf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnnrmzu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pzjtjrit.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ovkjwits.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3iqvqsmlb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abhdgjsb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3haxkfdrt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3frvtawmy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bpdnynpp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3okobqpbf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nfqzskbc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yipsblki.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kcobounw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gnoidjwd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bhpacwve.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ijuoxory.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gfdbhevo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3khyfumsm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3msyiznur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kdzpzzfv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3aotmsoou.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tberqgop.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lofkgnjh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gqknjcjc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3juqqrucu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cfppjqaj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsynlwaf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ycgnhsin.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bngiqzcm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gulhahrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aiwiblej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3keyvfbxm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ybwfjixs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qxamveqh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dazmdyxd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wemhjuos.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhyphfxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kvhewupd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jbtyohpa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3phmubrdc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dlribsiq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xgaqlhha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdrqponp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3szepydin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcuybfzj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ualnntgy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uelomdth.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aehkmkiw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfffnlo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ptuxehlq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3spypkfcp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pwlrkkoe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sudeiffq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xvlemtba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qenbmfih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxliwaa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rcwipxps.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3psrnbzgf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhzpycip.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tgpwgpps.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxkmzuf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bjjszyxo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3swxntgkn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bdlevjap.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmulmqeb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hbjzjevf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yngsovbw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3afjljzoc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jaaqfhfu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hotcvrow.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jinzbtwg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qerxgfpe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rdexcliu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cmweovss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kiiredmk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtntzaoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xtbdtwyz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3chauctsg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnjrpyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3puchrsub.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdsjpas.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qvjehctp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3erpslrvs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3etslkdsy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rgkjcwaj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rbcreaee.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wqennvor.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3syjiqeec.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gldyhjcl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyjwhobq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngmacxzz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dvjjxscx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ooaxapkq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hdmzjrmm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iepjjzho.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jouhewge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lojbjetj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qtehwfwo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3njrqqiev.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tkverfxp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cwoezint.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lplaelps.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cdtpshrr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qdbfuise.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lqpidmaf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxsfvc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ptpugkul.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vxlaktcx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fnadkuhi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ruwodhkm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pqhianlv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wmapcfbn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dtbsrblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtyefpcc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nnfetntg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqqfixln.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iijjlqnx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wqjigzkl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akepsjqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3eohukpms.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vkijikgk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwqtzgzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lnlhdmfo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmnofou.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cfdrxqfh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvwteabg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3whesvmcx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3algznfxe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jyhatnih.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbtwqkli.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwdizhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3eeldriya.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nkljvgpr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqkkzdv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lxtmczfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hijbiubr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3adgmguas.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sjuyyvpp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jjtkdmhh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3neeqjeia.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuwitrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rrjomtkh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qtacnsul.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rftjedre.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jqdliwrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eqamufiq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wfowuvhc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhnhilkc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yxbthzca.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbwfst.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3unynupeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vtzfofgh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fzdlwifd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ebagemxt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zwhouelg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbxkayjw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwefjnah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgvwljjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hyvcueqr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzgntths.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciinltws.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jfypigkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqnlnfzg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3spnlitft.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stvghhmh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igvbbjnv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uirtjmcj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbentzrc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzhomzc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rqoyfzau.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3oehandpz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkslubu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sngnluqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fcdjmswo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cneohpsm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jtccfwmo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3knslwhfr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vnwnsnar.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pzqqgsta.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dluhwfpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vlibtjjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uflsfplg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bplrerkl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xuwolyha.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ghbxxepr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fvjjfytw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lzfyowyw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hgolynhz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ulvjvexk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xujhtsik.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fweyixln.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3egxswois.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3luhmisjo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jegatfak.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gcfrddrx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhuwugcg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zljaepfk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kwfrcmzu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyzgigxx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kijziyce.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbpcznqb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpuavujm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fnlwcqol.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wolhlxgk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qowwydgs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmgqmlj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3srlnipta.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnykyjnn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzutnfxf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eawwinjr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xefrjvcg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqcrnwld.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ovvubhce.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hijeofex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yofqjfac.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jstwybyq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjzfuhq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gvijjarp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lawdixap.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3imewxwfz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3myphgoke.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3miovwfkz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vmfxysrb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pcooceyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdnhrynf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oxwqcmck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnezmtud.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xricerpe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tyyrsjfr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3owwzctmt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zjdbksmw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3axutxgmz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qmrqkqne.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3faqoyrqv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3umokhuup.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zilsjxwj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3etgoxgxj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ehrfrjba.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wkoyjggj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmoswgvk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aifskdkw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3viufedvr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmifqdq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3unlhlnhz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uincfqlg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lpweywrs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3parfvtxw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zphjaxsk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jnzqbqsi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gakpxwpp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3emhlnycr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vebaezlg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3stsgznrl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qpapxlaa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ecjoiusj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zbqxfzpi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3glvryinc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trfchbod.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpxuorgh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3plzqhack.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nitlciaz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kayzosyo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3badqjubv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wslfcclg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nqkdihmz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlrwmouf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3riujtaat.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxzgjwkz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyixrhsb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ucjbfftz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdcxohbk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zbyaukip.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3esfpcjqc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tqokdjle.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqfafuxb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axuhgdab.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qzcdopzt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnpaqpqh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3czhcmzit.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mpjjehzb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tcelvyau.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dkemfnus.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sxhigxtp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zugixfao.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xcybpcvl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fgzwrcik.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3znheibti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jexkoxap.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mxqzguna.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3swwthqrz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yafhckby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hbnowpve.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzglnhzy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xphbxdhz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3aziivtoc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3atjjskih.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bkebtevd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzjiaadl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncxtlesi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vdgjnvat.html


<!-- 参考信息 -->