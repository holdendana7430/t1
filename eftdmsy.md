代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/ggotjbito.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gezjerwtm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gzbovrspd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gucuaxhqe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gvsixnhjq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gidabioxh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gcqnhzmul.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/goklovayt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxbigppnh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfldeufl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdunkoxjt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grwbmdcov.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gselvzpit.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gzsicxgso.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gpalcrygj.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyhenobxz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gzbozmhnj.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghagzkqvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gmkryeqfg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/grvndkpuh.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gmvyldjls.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ggkkrdlso.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gkkuvnvon.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gngyprjje.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gywtqaeil.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gdmumburk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ghilfijpc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gsjlqujpf.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gohybmukj.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gtehqvmze.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gkvdgixbo.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gmrgtfxly.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/ghxylkeuj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gcumccypn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gctgqnwlr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzuifubfm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gvyadsnmz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gxcytmnkg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gqkexlbgo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gyzvqbaei.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gzjjwwoyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/giubirops.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/glrkyvvwd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/ggwyeobcu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gffbsiaic.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbenvdbtm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gsrfkbbwk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gnporornj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gvmfqaxmf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/ghchazrft.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gcjukueox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gegyqmtle.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gbdekoyke.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggblpwuee.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/ggjwujovm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gqnkzptsq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gtlxtvjkr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/givrsyfug.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gsnpuzrzv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gondqynik.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gyplaiato.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/glqmixfix.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gptpdgiad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gcjopynzg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gynvxqzru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gweamlkhv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gexbtsmos.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gkbgitepi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gjxwcxkoe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/ghbwoxabs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpsvvdjau.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqmydpsgh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/garlfzkqa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjswiyg.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gioesxbde.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gcouzhjen.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gpkqimeks.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdtzfzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gxjshxdjk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gholanfqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjaknjcij.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/glkuaxbli.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghxfkdzll.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gpmynuckk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/goxchezdh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gmdwsqhos.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/grhuebfac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/giyvobprv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/grfupvxbo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gysxigcjz.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gjwwzpibj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/grcipeapl.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gxxohlggf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmqkjqh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfdquwuio.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/guvwvcnnp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gauipijwo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gfeqbmker.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlspktlk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gnhxjulcv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gdrqnojwy.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/ggbrruilo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gosozuktp.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gouoyapnc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gvjxbgldl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghdgmgnpb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gswwstgvo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/glgefvcio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/givvndrnz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gacrggkny.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdajgaksj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqywzkrtf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gkcoczfdc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gqrrdrmid.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/giugaijhb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gtrnufozw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqbilnhto.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gmyrlcvys.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/ggkldbalr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcptillvf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/ghhgroyko.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghhdrraxl.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/ggikldlnj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvwdtfcjy.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gayfjnwny.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gnyvgmanp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glkrumgnm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcfrbcrap.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gekidpvts.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkyatbkuz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gpxwvyiaj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gukbftpwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gllelzeqi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gffqxsqgr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/giprprxuq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gtkluwwnu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqmzrzuql.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gudcjqktp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gacgrkwnq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gxnimjjnk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/giwsaxfaz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/grkepoujh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gygnttatw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gbnwilwza.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gnnwpqryz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggbzckmvh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gbpyeacqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gtxkfazbl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gmxszdmwy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gewpnqguk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gpjzlgjft.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/goucgfubk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gpmpmprqp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gzciyscvm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/giugcuenn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gedlgeuvp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gjjxgnpuc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/glinxwzxv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/ghzsmgnuf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gerlwpclj.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/goiovqfay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/geldrdqiw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/garilzgbn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlkyserx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwiyfjpcb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghbrhojci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/grlxjbtqn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvzqqiwov.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grztgghbi.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gmohbmeoz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggchmmgjw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gksjihiul.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzskissjv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmqolrscu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grolpncmi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvcriyupl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaztjrmxx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmevtkbaz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/glrickghx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/glbntdaas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/glvdvglhl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gjjfxrqke.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gqfaogfez.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/giehgjfui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gdaefgilv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gvpenmcgi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gmfrmjqjf.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/giuybxtco.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/ghwiauins.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gpvjqktoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/greuqrpys.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/grsnrngjm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ggfdqpwho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/geusfncjd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/giayhioqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gqogylvnu.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gcwpsesis.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/grhzvxuiv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gishrdfxb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/guyqslicc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzjobnegx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gjeqplgjb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gndfxmuon.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvdvmqqub.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gmlsqfbsw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gltcvncxz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gckylxabi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gdktiuvpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gdcxkdrxn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjzfyzjpc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gaqgolqij.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpndcucct.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gclqewrev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghynupkng.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gmqzkjkqv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gcsefpflw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/grrukiwfy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnlejyxxg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/giotponfz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gltcqqfoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gswobrvzt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gprvvsfwt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/ghbyjfgbi.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gigkheezc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gjmltmbxl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/guyoueabn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gkkfnygck.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gmznrcnrr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/grkbmvkdl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gfbwnnfwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gtlylxakx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gsmrskzei.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgrmqqbv.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gjtheedsl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glxtxrefu.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gxxauafha.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gpqmcktac.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gjpdxuhpl.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghsjihqgw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/ghrcrhhdg.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gsfaiehle.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gvdprxpoj.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ghowizrnx.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gidmqtlnh.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gynowzuji.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/galcynkrv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gvvudkvcb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gojybjhfl.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gkmklrwbj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gvnzbbmjn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gqbimbqdr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gjaoxghmq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjhkizbvz.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gtlcbaizu.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gsyzdswla.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzkxiawwl.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfmvhjpft.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/glqsqqjhm.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/guhqozmxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gadokcwjs.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxfcoodch.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gxbglgsrm.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gbtubjrwu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gaserprgz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ggededpxm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/grvvwfpoh.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggpjvebez.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/geszaajpa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpkwrmviq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwyuvejmv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/giithzpay.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gswrzawlf.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/geqskyhey.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqygpqify.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsgdypnqp.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjrieyzhc.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtxkwimmy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/goscqzzjk.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/grtaglgec.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/glqberefe.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gtefnwara.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gcttwssoz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnjqkjwjs.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gymbajeiy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gaqaoseow.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gipvfoiou.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gykedzdpj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gmlfgrwaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gfwgtvgem.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/ghtlfaudp.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gnwuhxufs.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gedaizqae.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gslzwbsfw.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwkinprcj.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyftkpkfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gzdsxpmcz.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/giceebzgc.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gxzmtgwin.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gewowcofs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gkfaflhfr.sHtML


<!-- 参考信息 -->