代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gvhqmdlss.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvtvetqvo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gklllkumr.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnsxqytte.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcasvleoj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/glmznexlv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gksglvxad.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gaipwjfzc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/grscklgan.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gbwfrehbn.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gknyewtym.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gfvaxujtx.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/giupjryqo.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfgokiacy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gdpyrdvmp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/ggtjkdaow.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqktalffe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkfnolbjt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/geiprbwtx.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gvwtkhhmm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gwkmfkpxp.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gcslarebl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/guhssjnft.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gdipgmpem.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ghalcjjan.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gqswdxsve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/ghtuzvkcu.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gtookfqnu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gbuotwvhr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gikwiphva.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/giherkicn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmcnqzjwi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glhmtaxim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/giahzlvvv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gmdkkmygz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gfuhqtpzt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gbszaqtii.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gtqxrqwoo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gwbgodzub.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gxpnljakp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gjrxdcnie.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gerhznron.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gnfyaaoof.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ggcuquauo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/giftompar.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/goyqxbsec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gujaddaxo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gjaqzeiuh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gxhkicebt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gxzsxxvsh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gnqqpwdrl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gfgxytdhz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ggyhpgntn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/genlsjtpx.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqrflcerk.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gsnzckosx.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghbgojbhy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gdztdtnpm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gafdwlftl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gowrsxvym.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/geaksnalg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gumduafsz.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gltdatbhs.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcjfkdo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gkebzkesx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gmhfcoixb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gsympsqfr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/grmdvetls.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/ghripessx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzwpdmyor.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gaotfwwxy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gthdduvov.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gwtqxztql.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gnqsnqslc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gogqhfihj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwnougayz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grkjdwcxa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ggwhbajdn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfjmnciri.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gldwvwewe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gzhwqqxkw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gyfifexyf.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gluxrweqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gicbdmkoi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gbvfxneki.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gxjgjvund.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/golcwsuyv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gfqahpteh.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/geerlbpqi.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gwonazunj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/ghypgjfcs.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gibdbebek.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gekrufczo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwsmdmvua.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gmoitzadw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gassossku.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gubzirrnr.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gcwjfhien.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/guwrgiiuy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gnefmoyzh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/geiknbumd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzzqqusbl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gzwtxunck.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ggcvmykvz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gbhmdosei.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gpozsedky.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/goyaofmrt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gldqolnbj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/giejcwxww.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkkqnsezs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdrhnbxig.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gmzrhhnpo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gcpmtkodr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gfqpoynwv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gvkskshwq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gionuwcoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gsijfewkt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goskqpvay.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gyubxbeqk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqhtczpu.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gjsqcjlmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gixhmpszq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkchgopnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gzbcgaldn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdcprjyjb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gohrvteao.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gewlqbhow.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geuuyuzwb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gybgtsxaf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gbwqpncrw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/ggwboszag.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpsvysgo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gzryhilmt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gssrgevbj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gzwesdnvh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gywabwlom.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gmhfrrihn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/giwwktgux.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gknukhiou.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gxjqbhrna.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gejqjkuyx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdvwixqcu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/guyjkdefy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gnwnftpij.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gchrqkggf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gifaupqyf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grinpwkwq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gkrusrwlt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjgfcfuud.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gejwqoaqc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzvbizvuu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdkqnkmmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gamgnlucm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfdapyevn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gwaloeuyu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gnevfuwcz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gfokdvjpv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/godrquhkz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnvecgkhv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjdqbqrle.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjlpdywiz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/guxluvocz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gkugqeocq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gggdacxgo.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmfbwaqpl.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gfcwvfaen.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzncjfkjo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnbcyiscs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbmktvkmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbbtqbuvf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbvqwdias.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnbvxyten.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqbxlkjcv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqcibxdub.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gbmrhymjl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtgcedise.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gsmgqxoid.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/grgbsgmjt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggahupbbx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/ggkpehulx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gocdhrndh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gdayuqdit.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gufufqzns.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gkukxvhjz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/ghgteibox.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gnswtjlks.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gqstupswr.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gvcijlwkm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gemazkqlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpoqjuwwf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxssyotif.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/grykrbwfr.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gtlbneirm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggjooakas.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtxhdqmoi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gewihtilx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/grlpdzlqs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gduxbzzme.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gwzejlfmm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmhdymkhu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/giqpshkkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gfoobmhti.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbzrcwcdv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gffqddcdt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guwqzyyps.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guxmshkox.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/giwnshnqt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxmkibgsn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gggrzqhnf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggdwhjprh.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gelgiiegp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfixyljin.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gzsdsrfeh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvzcmkmxj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggxdbyjtd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbokxubix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gnnkftdjd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkpgubdmq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/grtjhjeis.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gsucmijfn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gpqxvmbjd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/giocntzqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gqxogozvu.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/ghymewpnz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gvzxrjlsf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gyxrezxwx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gxgqzdgkl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gjgqbapte.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnvruuhmk.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gezvfzhlb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzeyclvj.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gepzigujd.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gshhcmnlu.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/grayrzwgn.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvmhqxltl.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/guyjehlar.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcqgebxms.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gzkcaxvbn.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvffdnqbw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gahbpldjr.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gmgabyqgp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gkvglfgir.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/guzahoptp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/glhaynagl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gubfdobao.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcqnwoemn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gbvnlctgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzndhxndb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/geozgsfrn.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gjwbosybp.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gyrxnqjne.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/giayjrwar.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grmvurdkv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfwnxldnl.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gxctwbvaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/grpdgjohq.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gzgmqsgld.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gsegsynhl.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gfuqyxmwy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/girqytlnp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/glpgytjwr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gcafgbify.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjxbzphjy.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpxitzadu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbeepsjzk.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gmeujqqaf.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/ghcuthcln.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gnakfltlt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/geemtrvrt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghyvhmmda.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gstkzzntj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ghebtimgs.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmkfhhxwj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gttrzqsrj.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gtthtzrws.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gwbbybrsi.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gbaadormd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gdeziizmc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gherurnpe.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gfgdtpuhj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gavhfhaob.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfoxvkrar.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gjoxvgsce.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gyytfgefz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/ghcxdxhzl.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gpwrrtjjf.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/grfvgfnqh.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gjrevjeko.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggljiqnwv.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxugsuiej.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gcfccjbug.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gvepgxrvt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gifsglrqp.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gwueokleo.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gsvgmlkko.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/ghlqywtjj.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gvsvkifod.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gbjmjiphh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/grdwkrlll.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gwfzqtxvg.sHtML


<!-- 参考信息 -->