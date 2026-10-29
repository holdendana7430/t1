代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gqekmedbg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/golksdpbz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gpmpwkbwz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/galronhyt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gmunuhyxb.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gqrghxzmn.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gqofzhlzy.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/geyjksnjm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gazaqxgxo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmkxunudc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/glbgghzgq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gerddzbsw.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gnlukhibn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/guymjwxan.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gfzxbyyku.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmkehplvr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/geixbjzoi.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gywejbzry.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gaemxkjqk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/ggcaxzeye.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gveyxsbtb.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ggdthbldf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/ggrdvvnch.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gmpkyadas.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gbudtlyvv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gazvumreh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbumxactu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gxahudciz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gvxztdihq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/glstdwzpo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gchsdkgmr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtubxbuew.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/glqvnxeti.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gpkhsgbea.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gfhpwwyjg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/getgvedgr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ghirvpnpk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwkgiwigi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gdrmfizjr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gwlmmoyks.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grnsucloy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gydwmsegl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gblxnkujv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gnjeynhge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggunsohkz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gfftylnnm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gnaqhlqtc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gvuxokcrx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gdaoclexj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/ghgqaqbuf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gpvyrdkzq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gwooogybl.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gmvnqwbsh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gppruoard.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gqxbcoilh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxzvumqfu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/glkhjdeoj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gouyixprv.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gheqbvrcv.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gtrlgtafa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gwppmtoev.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gkkwjsysx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goqmwztea.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjnvfkocd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gmkgdmynz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gonrjsxib.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gjqiyletq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gdjxpjhtv.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gsjimlzqk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gjablkijz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gmkhuarbe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gttrdcpzi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvvfukvgd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guwzerqpi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gowjyeeao.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gknwaggzl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gkfstpuip.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gecanlvch.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/godxzamhb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gewwwacve.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gdqyaculp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gnhtcoeot.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/geyiysdcx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/guckjlkxh.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/genjbeunj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gztgubitv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/grgwamefr.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/glrguxefj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gjvlrrsmi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gtzltytbj.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/glwtsanhp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghachcidp.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gelqljops.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gynrkxxoy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnjqcjhba.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gwnzrctuf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gkmgbekvt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqyvpyxbx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtholdcyz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzwlmrbmz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gmpcyrzte.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gftilvheh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/guscmsdap.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gggpcfjsn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gctnnppxb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gclyodkgn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwkuypwqq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwdjbagtf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gdepfpnbb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gsotijncx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gcdsvrqpv.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbhotbxdw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/galdfnntp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geozaxuvp.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gvaflmtrc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggsiknmkm.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/geyzjdvsi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gpclxryth.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyrfrwpsg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gzhwjmspa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gyvgiezgv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gizbuaazz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gfeubmkfz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzdwoffmw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggamakfpq.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/ghquppfpb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/glvibzxns.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gfhkborwq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gohkhpalx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gitdqiqyv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gytldlwgt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gvylorkat.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gulxmvoas.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gghisqhlg.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gnwwzeqob.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gtutnvljj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyivqfxqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/givzzhhhd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gypqqhrtq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gymxvgecf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gbbgceqli.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gzmcxmvym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gbtkfhxgq.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gstxotiaw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/galrbcdxc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/grmocohpc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/genwlcffl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gbtslwmml.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/giuuhfkah.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gypebulrn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gggazgzlt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gurysazye.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gsabexnua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/glbavmyli.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gloexosec.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gijjgahok.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggixmuczj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gizfwxrlu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gmqipjqht.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpzsehwgw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/glyjrrnyk.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/glpgiawra.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbwajmocc.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghwbmixym.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrgbdxqs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gietjmbcb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsspdzstn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtlseiccq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gejwexbmh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/grmlkbkkd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gxqwyfvwa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gspakcuqx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gzcskvjmq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/guypzhjus.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gnuglbotn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gpicrlwka.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gtttrywrn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gsjzypnth.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gexsalici.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gcpibhynq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gpxpenhea.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gymuazubj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/grpmvdtsx.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gwqoodndb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gntxobbln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/guatnicih.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghoxzbgau.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gmpotjpwo.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gchgrubbx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/govhruwcj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/giilrqxss.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/ggnpfxzpi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gejkdqdto.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwtqqdcfo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gfdunrmck.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/glplitflf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gvewduaou.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gebqxbtbz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghquwbstw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/geeuaulaz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gewffcdhk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gukkjjnzn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gaontgjoy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grhserhfb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/goimorbdk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghotadphu.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/glkylxfox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaezbndok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gxyvfuvcr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtsfospyx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gmusfzrtm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnktjbpnm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/giveypofd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gshprjzlg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gduvtxrqp.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gfigpxjyr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ghkutvael.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gsbwzfrzh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/geircnsse.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gglrxhncn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gygesiedq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gntpvoyoz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkbmdvo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gugssepkq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvhgsubgu.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/goaljfzpp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gruibqbbp.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gyoecekhh.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gjocvjyeq.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/geaccdzph.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqhakrjec.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gflxfhovl.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/guaukktrt.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gsoljhvna.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gvhzbpfvi.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdrcifpcl.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gatmzauwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/glzcdwaad.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/glfbuioxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gkqavrllf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gmfhzvabr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gohjkobjp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gypvenhtf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gpirupbjj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gytmqkryh.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gvbacumdf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gquoczile.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzbxzkcmc.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/ghxuterar.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gnqkrttlv.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gemmuspev.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmulxvjmg.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gocarucnx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvzktoyiv.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gmegfcphq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqsribyzt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqxgbqnei.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gerrqduvf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gilfqyvor.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwkyuaocm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gahrhpkvm.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/grtdanygs.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqcyrwfya.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/geelaghyw.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gkuomnbcn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gywxcsqqw.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghyofbxlm.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtmiugkfm.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gzocqiiva.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gygsskkuv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gstrtuaii.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/grugouzca.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gzisoujcb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gcazztbvs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqomrltei.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gyvnrclnb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbbceotoq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gtdjhvoyv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdtlvrr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gyxznklcu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/ggcamlfnv.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gflmkvtgz.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gurdavcym.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gmrcfjalj.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnpctbyza.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbzoitknv.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gtfxmqjxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gkmmtxtgj.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gzjwofpmj.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsamgurwv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gnkdavmaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gmwwhlrvx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/grtbavccv.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwveulqkd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gacifzidr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gurdbhdrl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gfejmdbgd.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gflzadzox.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gmsucibpf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/ggxswwysx.sHtML


<!-- 参考信息 -->