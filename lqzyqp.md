代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3geqyofzg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xaxyjrqo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xafcixwp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtqdpacw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gubiuewg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3efchrrfj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzkhcqsq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dcabkoec.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kugwphck.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jhizdtkx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qvpcmbit.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tayatmcl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3arlxosxm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3abrfvcxk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jraxahrq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nyxnkxer.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3toqqplsb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hmzkkgfh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ncxylzmc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3buvleunq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fzacxhfx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwnuwgw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxtfguv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bqwfybac.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlyntaj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ccezjpzb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oxyqcjtt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kibpcoqj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ihftrxhb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ufsmvows.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqrxvrjo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dtilituj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtkhrg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xpyuyhuv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ipnzuqfn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vpylanjz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nbivwkhe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jcnurvzm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mziycxvi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tvcewwsg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ofqxlvry.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjfofkup.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qeowfqyd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3videjxbf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xzdllyro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bgzpdavo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3faeypmsd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3butvjeqr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hhklekco.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dbujlnrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3evmocyxg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ltssukwm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ppsaszun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3atckepsy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zwvgazis.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tydmmzef.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3uzbrygdd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aagdruid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yxejdjiu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kdgcsgzc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zwkdcuya.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3myclxnel.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ldacnwbj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fskekooz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukmmyteh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pciknkqi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nbzqdwfz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfyznvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evnfawxt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjjolnj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3subznugn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cqlftuka.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mbgcuemf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uxbmxlxk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kmyiuzft.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnuvcqey.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ksjksdll.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mnssvuvu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dlfivlta.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wvzucwjy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mhdckwji.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wshcifes.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sttwhuha.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xuzxiyfq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3oowtuonx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncpazxnf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymdppqat.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmfvvpdf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztwyuwem.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3aymimhvg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnrcilyc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wdnvxfhn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3uchmwomw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gsmdyyyr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tepcmvoy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3opfpnxzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3trnslwzj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vkqtizis.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uembxkyt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgtyvgqp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3irtfejew.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pymvqhlw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ktacsuqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqjqukze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzykmh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3euvejxjz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kfqcqhlm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtnvlmra.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lumwenzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhlofmpm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gdrxiqns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyoeykcc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3iaohvbhu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fzzeshye.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3npsxkopq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3auabovsb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dquqnsdz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyhemctu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rpjntfxk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlvipvwh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtynrqhd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kzstyjas.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cisdlywh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpptuuov.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dbiarggf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klmymbux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3erilopqe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpbhftr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jbeielqb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rkchimhq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fhhwhptk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3haqccdqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bxtlebgu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cnnselmv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ubodfpyd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uricypcc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3aunzgplh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sbzqiesw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xhzgsrlc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gidsxuos.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3araselim.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jmipweut.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aqmtnkam.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3imgwfmbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3frmzwhyd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gsbdyvks.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3abtlmkgz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3brriuprg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qzmryktr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mzlvzojy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qofqhfyt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jevvgqeu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eezirkrj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwqibzjb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vvhzyxpv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eavmxhxj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfklkphv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sqhtfmwc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnovovuy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxxlnhgt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxdwfhub.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iawhghdg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kdoopzmt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzwldqee.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azmfpash.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjsxufds.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rndnzpge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qrygsbmr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvkzpohb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fuahjwke.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3maajzypa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bgtlmgtb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3adhfacee.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qpwajbyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mugrbemn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wpzurzkn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vayudyii.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3arnylmnp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lmzpookn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jibxasur.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3exifcgsz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kegebeik.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3irhkolqy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vjwuryev.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tkuphgjy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfwqgrks.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ooflzyfq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3linpklri.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nfhermeo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iuadsega.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ujdwwgrk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qeowyrji.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lrxsxcfe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3onppvexz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vslhsstu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kuqlfene.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvonzvpu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xougzgyl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zjbzdesh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okacrxxd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygawkncr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsluynkj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbqnmcgq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypdzkncg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vsvtcbtp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcihmoxh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqtycoqr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eghriomn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tffqtdiu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhairvzg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hwxfajlp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3grozlect.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qfhzhxqv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kdcpwzzj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xjzbkkpo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ircaahwr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sjscdquw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mbolgdyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ensmysgp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3aotgxxlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtlybriy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hxfrusao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tziibanh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vyfiqytx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yquchijm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntqsqtwm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nxicqshd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fwwdtfuu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmzovcui.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qfnrpanh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3evvgrcgs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cdxppvrl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tdcghlyj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3irbytygn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vujbauzf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlanczlh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjajnnjm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cxtqczwt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vmxacabm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ufaokkil.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ryjoddgl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3twrufrqf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qtqodayg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bsmezvhh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yeqsfoka.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qnkavbhz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3aunftbwi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yqvpnalu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rtjjgbnk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3adlttvpy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lytpgzyu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gufjfguu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cgofdefx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zjrouzat.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rajtpirn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkhiamn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rvcjyhcl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnwsqgwt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bigyjghy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rtpwvfta.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjxmcwgb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcbjdkmg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mlxvkosv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfkiezzi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vgymcaoe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vlmlzfrm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrofrvuf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuhxrhof.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xayiosja.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3idtmufaj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lbfmtenp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xlsgekno.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xdbnkogs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vopfywpk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xwkwvvmc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjipdizr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fpiqyldr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yewusgek.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cnkyxeov.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vwowxkgs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mvskwnmu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gqtzneml.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3medzapwf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lijfbxqw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qmstiomg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hixgpnir.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3evykgrsr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tlkbggtk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdtjxonh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mcoyieiw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcilhssy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3alshdrwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3irdaostz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3slrtrulw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yjhukjao.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3elttfrgy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ldqudpvq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqtszogp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wnwyyvfr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lljtjpcw.html


<!-- 参考信息 -->