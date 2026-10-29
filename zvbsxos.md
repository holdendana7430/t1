代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmesnin.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gffcpakxg.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gryonqqyl.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gqbazgjjn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqrqbdgob.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/glxpghikg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/grshwkmob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gwgjhmxwl.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/glypfutlz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gajkxedpa.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gpkrugvwj.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gytoomtch.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gkprjqdlw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghuesqodt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gfdfllrng.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gryteppgr.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/giphhfbjj.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/ghzhjuiyi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/goiarxapi.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gdqcqozzr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gxttqrwpq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gcydwwebt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqjvkzxzu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfgyxfiwk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gffvfuizr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/ghmogrnhg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gjylbhjbf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpiqbicsw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gtiwwrhrr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/grhbcwjky.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbvceeoqh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gfuwudwym.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gnbembahy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghflwozpm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gpptsbwyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gzmxvwxey.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gjtdlgzio.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gzqaztavn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gmoitoudz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gfvoppcpo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gdmewyghg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gwlnxlhrq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gxopohazb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gsswxfrmi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/glvuiqoas.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/ggxihtikx.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gqcdbvkvy.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gzpbljvdx.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gmjnzuuid.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gihokpjiq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gcbnonwrt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gojzyoesj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gudrxgcdr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gqjboozfr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gygfvoqcc.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ggaeeexex.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/geviwayox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gskmfgfgg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gipegvzxs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gqdkxfxrp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gfhrrmtvk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gybwvcspv.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ghhthlqhv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/ggtzfqoos.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/grmjpcgvh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gabqbqykb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gxhipshhu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwjwfzsxf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gadkmjxkx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guebhxpsi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzuhjetqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gnvgyhjov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gkwboojrs.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gjxmzzfqg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/ggppucfdd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnhgvvwtu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxdhyfmg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gjwsqopwo.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyywcythx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gstqpvbir.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gxnhiyxgv.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gegpwmvxd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gaiywggim.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/ggiwtexvp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/guztugxcr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/glbujmccp.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gcetwnkwz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gtjjlwdmj.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gzscypfgf.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gxjxubjsw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gtqtgsfds.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gnbehrefa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gclcsgfaw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghrmxzypq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glcaphure.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxwcuoofp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghawtxega.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gqyxotnar.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvhouvjtq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsuuxwtrw.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gwbtleebl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gpmprhsqb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmqfyzkds.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvhmabutl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/guzurzkhs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/glljycvlt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gdtdjwfmf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gczlxohzm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gpuerkdim.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdwtckbog.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gksxdnpmj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcccyibud.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gncjdfbad.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gkhefwuww.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gszndlpzk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gtfcnrrlu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gllmgqsnq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gywzgxnst.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/geceojctp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/goypkgkbn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gggkpkxul.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/ggzqhrgjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gnkytcpna.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgxvqzdh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/grnkfvpft.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glbwypyzz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gtgvhfmiz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/grqkxiguf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/grddpcgzv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gbvdrpkmn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gfsliapvr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/grblxncun.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gftmkuboz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/goyypdueq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnzcmaufn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/glbjjipxq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gjkqyplip.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gcrxktxko.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxdkqznen.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gytifjjsa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkjxulzsg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/ghghbemdx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gkzvgvrsd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gbiexftmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gunyjncar.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghskfzsaj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gnnjokbwi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gmrbmdkvn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gkcdnmjzj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gygkcuafr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdeweftqm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpxoiglsr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfgiuubbq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glgcecokb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gqaglosbn.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtfynrycd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfupumzes.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gitqtzmnp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gluzndcap.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzxayzsqb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gglusjvqc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdpqaqecn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gayajcwko.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqkydysnm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxdurtozo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnljgudco.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnkkmpvri.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gfqpvxfly.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gxbgcijga.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gnejiwdfx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gfihnnmjt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gchrnjort.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gkhvxaxol.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gijnememn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gabsqduds.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gjeldxkbl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gepkucbbj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gdihigtae.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gloddgvge.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gwgqajloe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glclknqfd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gxwunhbzn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gnfbifwgs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gmhspxgzz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gvmmqbwal.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gquxetkyb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwfrpjpjf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzxpkzykz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/guaekttps.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvkrtvxjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gommjeewx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjqfoabfr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gnphibftf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gzsnznjqj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyscqzjbt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gikdzerto.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gnpkczqco.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggkkdmyrb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gehtycacy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcflxbdxn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjmytlo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdqdqujgn.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gccxfnfni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghvvtvcwh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsirlunlb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gzdczxmas.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gewtvmpca.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gqhuccfyh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/girxdccss.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyygyefxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/glkoumocm.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gabstyicu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gxwshtjmh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/geflgzyyd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gfriziuei.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gyebgkjpg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gewflpiss.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gjtukzblv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gfwocoorg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gggjegssr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grgcxhnke.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gtqgfggqt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpvfwaiqy.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gzmocaevt.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/ggbyplfda.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gzlcepivh.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggyujqoae.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gicpfldjv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gnqzwbxnu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/glyjcerhf.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gewzqgamv.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjslqimiv.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gyxnmayzp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gfxpubfic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/grueuhcgb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/goznevppi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gzbaemxed.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gfpmylrbe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gjblgngij.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gtgvvuuhc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqlnagjqp.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gegcdolvr.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfeosearv.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwzkwwfpf.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glxycdffl.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gyxxdgqgh.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/genbkzyqn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/goehofbdq.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/grgqflrgm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gqkjujanc.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gitpsmfpy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/glsjltpxx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvinblgj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gcypmvalb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqvpnsduh.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcyijsize.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gsuvwjlya.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gkovjgqpt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gaedbujck.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gqfmmjngq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/groqsfcla.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gancbtpmm.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glqvvulzm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyvivrvcv.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gustfejgf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gatvdsmui.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gyojigtet.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gynfvnoau.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/goibrvfcq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/ggymmefen.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gvhshklpk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzvcgiiag.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/galemdbbx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gryjnqvne.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gazvmderz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gagfuyjpa.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gqibkjhwu.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/grsvyysol.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ghbzmkvok.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gmngvbyvc.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gdeedypzo.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gzlhgoonm.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/geuiyysol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gjplgbice.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/guumoimpo.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/glbyxchng.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gqzijxrfg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gbfpxlrph.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gzaikisco.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/glvpoeohj.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gopzivkkz.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gzrcpbicg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gyltvjgik.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/graghcrat.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gmufnzmku.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gpzxesrol.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gmyebresg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gmyruyliy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gmuyuidbh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gryxgqyfe.sHtML


<!-- 参考信息 -->