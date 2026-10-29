代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gsztukrxm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gscnadgfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gstwtcvwc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghzbbbelq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/geyyvahea.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpaknczxc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gpqybmmxn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gczcyfvcu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gylihkuho.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gmrqlidnn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqqmqywie.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxgqrdxza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gwzedyxlu.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzcehda.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gkacbvkbu.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gttcnxscf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/giwmpirse.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvjjumikg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/glhwtvgsh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gbzdstrum.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gglrhhhbv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/giirqygpl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ghsjzmjmz.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/glkazabvu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/geqxmfhmz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gpnytxqqw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gstleeygt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gnnoinycy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gmpribogh.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gfztuwdbt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gcsnijamx.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gpzuudlsa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gzylorszk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/glnbzkhsf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gipestomd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gciodtzbu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gsesvxoyv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvlgxzror.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gthpivgca.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gkzoarvbw.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gprupcgiq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gcuaxxlhd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gguzbkptd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gfyofkbif.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gnlvpatjm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gqcqjsrwu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gwshrxuxs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gheipufoy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gydsslujp.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gmtiegatc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/glkhzxadt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjxgkljuh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gmrvvpckp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdyiucdyk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gvlvfcrgy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gxxvdgggg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/griqaogso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvskognbs.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gjlvpceqq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/grjhyllip.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gczyjvroe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gegzcljxi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gtwfmoucr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/goecxgnph.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gixiaildn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gaqlvggfi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gigjqmyun.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/glbjbqmdp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gcaetnbsa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gtmrjhilo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/guivjbpcd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/goyewmghy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gstwaktqp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gxuolkzpe.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/glhabdxjk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gyetwkslx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/grofsybxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gwnzoljas.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gayctnslr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcmvdstez.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gkmjlbfho.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqykazwjz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnoxcfjoy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gjnxoiajw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gsrgshppm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gsuqgdqhn.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gidureaxw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gkyvuqwmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gkilecqaq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ggvjzzzsw.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvibzcrtl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gsecryvbi.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gugvabxma.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ghcyaydcs.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gcyzjdijv.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gvpnpitbs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gyoqnbzva.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gpljdccyb.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gbxwwbmvq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gakaxfjdz.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/girfevtvx.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gqessyikm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gcxaebhas.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gpyzbylfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gghgyehnz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/giugvnrim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfninhspx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/grhefntsd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyzqunhic.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gnxiqcazo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkqraapeh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gwksnslhg.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/glmszvfwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmuyoocup.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gclgvyyyv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gnybpfrrg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/giuwgkdyn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gzpvbzrdi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gceekramj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gvawpbfts.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gaahcszsq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gurenbjli.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gnuiexxwa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpiowzvuk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gcnrnamfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gcacjtnhc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcjpmxtwq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/grjumpqkg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gkihupfsm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqjtynjpf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/grcnmhzcf.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzxofvmde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggdiypavh.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gofcbzhte.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gyhhiwiyn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gzzbmqgbe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gzyuvtuwc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ggjcrpinq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/glzlwafmm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gpqlknciq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gclburxcz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gtkjkdrtz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gwvomdfca.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gfsqaesxn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gnlpaqban.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gykdvsewy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gyvortfoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/ghpkjsree.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gjibpjbyn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gbzfxmahs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gdjfwuavb.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gcboxwwak.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gkryjjsil.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/goffrdsow.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnbzwudkl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gueqhfrbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gpqgekben.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbpquwhrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gmcdglubq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gavjithmp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gblvsjmtv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gvcqarhsa.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkempfcny.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grcwmrjcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvgvigkkr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmacqpeuj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gfihllkhc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geoglsqvd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/giahmnrlg.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/guyjzkwug.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyhykzvbx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/guyssnrrp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzoqrfjxm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gezvwkrli.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gdbidjomt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glmzwghnw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guubuapov.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/guigtztvc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gyjjmqndp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gavgbgpxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbmhtphqd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gcsefkqbt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gazfvocgj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gjvgeqbdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/ghwzoelly.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gdhtpbqzl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gvcfcctla.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gwzslkhok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gbloaqfyp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gsooaeryz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gtuysivqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/giyxjqwsj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuotexkd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmwzafvo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gzoitvijd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gyvduxsgq.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gxubcduea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmpxhngkj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glmfkammb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gpewzgoqf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gfgadfwus.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gfzxisnfy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gokqswndg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwskphjd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/grbxxvddd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gmhcitdwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gerysgiyk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gktnozqwu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzeidycpn.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzmkzjmwc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gnqdlpdrf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqmuwkpmx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gslcjgbbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gpvbgivgt.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gqrhhsvcc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxbrylwkv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjfckapsp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmyrktsbc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvvdgrjoq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdkyklrws.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/ghaiqhwxv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gpmmvkpwn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gztimxwxx.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwkyyynih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gygvcmnqj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/grejiwrno.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gicmdxniq.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyruksh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gflzksylm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gxrmzhpuh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gzuniuowa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxlwkcypv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbczqjxxs.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gppkiceux.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gshmsjhjh.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gcjexplur.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gclrigruw.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gdafifxxe.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gskrbapko.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gqtcsozsw.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gqbgadxfm.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gyptfjyqz.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gpksywxdh.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/giexzpzle.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gvwxlgckp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gbkuzupyf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gnspobtyi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggqcpgaxm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/ghzulkeej.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gcmdixfht.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gexqvccds.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gupbjhrnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/garzrzjwq.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gyujftahz.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gpxeafqak.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gcegudgli.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvipdar.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvjamgozs.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gmtbehoht.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gzvzfaruh.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gtuvbtpoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gzqdcgobf.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gqxcjadhv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gmvbnjnms.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/grogmphhz.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqargdlkj.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grsqyrbxb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzpfgbfx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmdsjhvcu.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gcyivlitu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gzqhnpcwo.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gflegasnh.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gcrwnosxv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqeootshi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grtybqjbf.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjiocfefl.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/goexicuwb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/guxtmkaon.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/golhrihgt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggujdxalr.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gfmxbmpef.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gyjrkynpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwummrlzx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gyjcopuvk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gssevyotm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggubjypvh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gwbnhtpfu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gztofxdco.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/geyrraymo.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/ggyxfhopv.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gyojxtgnz.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnjhyeypo.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbuicdjuy.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gthlorkvi.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gwopcrsqn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gxgecjzqr.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gysuglyje.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gxykohsbj.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gntlzaafn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/goqmcdzyn.sHtML


<!-- 参考信息 -->