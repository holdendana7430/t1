代发 wailian999

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gxyjatqzz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gghtjtunl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpyrqloym.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gkcbwduxs.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gruudzwcf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gsfiiwyvq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gsubsvcvn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gekibybnp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gixgaajov.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzuovlhcj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/glpejgkie.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gwnjqzakl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gwpuiskjx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/glglgzxnv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gccpmjony.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbietgywr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqpflubvu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggyqlekkw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/guvcdalnq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkinfamyj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gjujwjynm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gvepqbura.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gwbepjsct.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/goilmjqvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gokrpnnlj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gyrwehjwu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gkvgfnxwm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gdezwpchq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/grjbicbvq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gslwfarqz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gitacyjyj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/ghzzcsfpp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/goblqvauq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gqempxlyr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gzllztkyw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbnydwahh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gkadzwapq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwngvojsy.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gsuyviqha.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gmorezhml.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gbuquocdl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/giaymxhtv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmyfuafun.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gfrulghbj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gxffeqdas.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gicnqlaes.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gevzihqlq.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gytqqlizj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gugglaqhk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gkvzxxgpb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ggmvveffl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gftmhguiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/glbpuesnb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gkrztwifz.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/giejcvueo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/ggykxisbc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gdftpuzvk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gqbcgfkmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/glrfugyst.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvnhwcn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdechfpow.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/giuczdids.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbukmhfyk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/glihuztxu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gprdzwdvl.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/goddkjhqa.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/goafbrzew.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/guynxzjxr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gbiuwxgmy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxtucwoxo.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/giadebrnk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/girkrnapk.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gqyjjtazw.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gslxqvqkh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gqbaxhacv.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gunsxovqd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gbazndwvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gszbvhudw.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gkalvdtbo.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gctvwqngs.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gzqkyrnmr.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gbrtgzpet.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gqlcftpng.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gkbeffryh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/glqudzurb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gburqdosq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ghlscgdje.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdobseqqi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gpyfebsiq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gaulvsogh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gaswcqorh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwefcaoff.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gjjexcfod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gamgowniu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gyqerxvsd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gquuxupqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/grtdifwcg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gczvmneiv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gaiciuswr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gpddqlnxx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnauiuprc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfcrthjzs.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/grtmrdnpf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gssptbwjz.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gornyqtdr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gbdokimaw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggindqjhu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gsqpqakfo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsoyomlfb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/golsjdlhk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gyaqfjnaa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtjckfevb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxshiaqjs.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gghzofvib.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gehwwruzl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrpcdgww.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gvdhvqdcq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gbqoyzidp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwxjijxsw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/girgtwdiy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gavguewwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/ggbobyext.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gigheclax.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gynlrlika.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gppxdyalt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gtmpddavy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ggmwosnks.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gcryjhjtp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gxadkmgdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdrexxdnh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gpifbhuxu.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gmiazhsdt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gjmjimnma.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gwsmnybwh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gakndptpm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gbdejshby.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gyabsrdvj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gmylplfnv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/guhazwndh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/glnyycmhs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gqaydgpfc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gigpfntlg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkiiwgoty.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcowvazxc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnabppygw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gogmtbwbz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gqbzlejrf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gohcbfjdh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geidmsins.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gccslqydf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmzvkeiuu.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbjeemeor.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwunrbkkq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsyijkwjf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gzvcscwcp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwbvpulel.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/govlvmekh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnfmpchki.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gdgrsbuwi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gkcnmauoj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gdagovlgj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gguxkodds.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grdrjyyui.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gskdsurqm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gofebzrkc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gjnrhleya.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gaddjzdxs.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gwlusptxv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/glagcnqaq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gvuumxcnk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/greqxuyru.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gekuanyah.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gyibwvhyx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gaeabmmsf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gmxhksktq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdtqdxinq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gbshzkqqa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gelyulghp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkkbnxvsm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdvuijgzp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzenttzuv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gaghyywwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gsocqcewq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggsvdwxxa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/ghbdgarin.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gotqsgcbb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggbxphwil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxbxivzjl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gfvcaendf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqqenduci.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gvapxukvs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjesbhbdy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggpsdtqhw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gijohzqgq.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gyimiyvie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpfuppkvr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpgpxiwrc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gliaxfngw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpygpoxlt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gysnbozwr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gkendigej.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjrrfvgvl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gxoyysylx.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gfrmjrrfy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gzlmlgdsa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gtkcnjvwc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gsywvwuif.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/glfsyflrq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gjdcsjspa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gwtwsvfry.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gevkgetod.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gcfncygox.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmgaucpj.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gqbjhiqrw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gykfhmece.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gveokusor.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/ghibbucgc.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gnmdozgsk.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghrpuujqw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gdjjobmpn.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gdbkjmwxr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gzwjovgym.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gmaopnorq.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gwhrsotqs.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gibwynyqn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/grdlxzvuu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/ghadeiabv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/grylkkurb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gtmgjsygi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gihxqnhtl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gpsjttwns.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gyinpszlz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnhlnnxlc.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gssrinoxy.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbkgvfidy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gyvwzcmtu.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gcblskddg.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gyrzexuky.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/geadksyxt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gbbmsosnp.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gqxtoekup.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gnvtpklrd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gbenopeji.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gldpqpenx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gawybnstf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtbfscsyl.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gleozhibh.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gymwufbcr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gsacuobve.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gawuchckz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gsouonkuu.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gctmvuavc.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gjnixttmh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gswyuulic.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gtxjgqlgu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzdhzcmda.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guiblurnr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gczcpdwwd.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gbsvbqanv.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gorkvpdlx.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gwwvuvvfr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/ghybdkiyq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggrcpxobv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grnyinjry.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbvsoreho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnofxhxou.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gibfchoek.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gnfntbjaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gklbqdsll.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gvrlndidc.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gzbyrtkck.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/getgkjlps.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gmlljelpr.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gtodnnhli.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gdgipfcim.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gisntujgi.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ggdjkkmvf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/ggilsrqqc.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gavjhvhaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gcjeqihhz.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gyhnoczjl.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/grioldfvn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgfxjlr.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gwrifcgnb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gsuesoelp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzccars.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gapvlbmgn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gavaqualm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwmemhq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gbyoqdmac.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gebeffinb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gwtswhffg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gwzusvmde.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gozqmmwtb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gsbsgcfcc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gkirxblzc.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gnslpsogc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gojfdaepf.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gvuavlbro.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gfbtaqkby.sHtML


<!-- 参考信息 -->