代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvszpadd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gsjuaaspd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gydbsilvs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gwlgsennz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gtejzgzqj.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gsbukbxts.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gfecrnorg.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gqhvbkvto.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gyrkbzgzy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwtongupm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gcxbafuur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmkgpnpjx.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzejckvev.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ghchismrk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/galmvjicg.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gohaakzcb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/guqkgwhed.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gbdwkancq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/grtgimymc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gashmyriq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gonqrctoz.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gnfwgxdno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/ggqsbsomu.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gtgpvbttj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gzpwxowvy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gauwonojw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxnjbhtwo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gewnscnil.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gulgwjode.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gyctqhlxl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/ggyajdelx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gugbmmkdz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gddsfquoj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gyylzigtr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gkbvrucju.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gqpzgbldn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/giognwhga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gudlcyluf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/ghtynmvja.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfbvpcwba.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gpdkmpaek.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gybznuvsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/geioapfus.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gbhfvgdra.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/guklgcijx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gtiyurhgy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gloujloja.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gxrnfklra.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpnqrwpzj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gyailxtat.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gudgsikei.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/grqcoooex.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gaigdaxaj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gwiwmbdua.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gzsxhxnru.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gynrwoqqw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gpwsrmwso.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gyyfwqsbw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gfxtoynkp.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gchaoubng.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gugjsvbzo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxourhyd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ghzshxkqo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gdnuawtcv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxyfegzqv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gifqqvxht.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gdsnxrsyr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gusyehlek.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gjjtkowxj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gwuzodmgh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gkmydwehg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glpbrotgn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwhbxbsrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjbqeufkx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbdgwungf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gvkfqcrtd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gmuzqoacl.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/grurrbjuv.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gwjkkfoiy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gqqbobjge.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gvugesjnp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gsinsdxwg.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gqdcjpwqb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gecmlxxis.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gwjvtwcsa.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gbnuqhjmf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/glttpzvek.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gfygrvmoy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/guoatplwa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gtotakiyr.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gwauwfbmc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvtibjjlx.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gozltijbx.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gtewbollv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gxbkyjurf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gbeigemjx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gpmkeasde.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gehmlorlh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gatkjfozj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqtipnygw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/govjzfahf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/ggzqcippn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmazviufl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gggfmgvmm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gentcllit.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gwihwrhzx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gibliqocs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/goxkhkbea.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gcdqnluia.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gvuqwsgbf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gvqzmtxcl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gvtqduygg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gfzvicpgn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwdmsyrmr.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/ghnipxcyl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfaciffle.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gjnvszuoi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gbhlomrmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjpaollty.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gnpfnepol.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsrlffjhs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gseqpgijg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gukggzdlv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbbpnqvqb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnrjonbnk.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/grmxigpiq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gthusqzau.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwzizdnbn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gfzyhbzjs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ggusrhrvl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gclnesydj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ggrhledxo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/goutywdcf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gldyjywwu.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gvakkrgmr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gkjeghaue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gthweyqvh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdcsxyumt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/girneykwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gizkqnqqo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gnfvulsds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gtkpaghcq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/glmgjmrxa.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/giyjcfwat.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gozvfwcdv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gtmpzjpvo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ghqhktbvr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/glhwzguii.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/grqjpeaca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gycqfvywy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gllejnifa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/geqdpapxn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqvefwtrp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gtrmdxeod.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmczalonl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glujvovmj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gadlfxlla.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzwjlirfp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gwfoczbrw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghyorwdim.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gldtkowgi.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/grrrehucd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfppmvwof.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwyuydywm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpxmpuwug.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grasnzhbx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gcnguqang.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjleqcumu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glbuqqski.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gujyxwyee.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gvtdgpdaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/grqljruwj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/grykxdvut.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbnnkhchb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtcajsdue.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gjxdzfeeg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gfvhvfvuh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gtlhdlrwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gnbmdoqiy.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvwmpypxz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/geeyqizlv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gyovtwnpt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtmqargwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdlpoxqoy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gamzbumwv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzylrac.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/grhisucfp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gfdsngfaq.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gnuarmnpy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gihwfvklg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjgvjcjrf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gfjrunqyh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvydvfgtt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gcadzsrvi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gzbwkumuq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpxkjmrnf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gkrkhudwy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gtpijpyhm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goxqozsxr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnqdvdsfe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsclavbpa.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpmhvmfxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gipbozcub.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsvilpktu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxmkzfkvr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyndgrlvs.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gqrlopryl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gyysxipew.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gohozcbft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwuhrvegc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggqmbdsyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghqhifbhq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gzqfuzxvg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdyyrakdk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/guypmbdvk.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gqevjmylc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/guobaiogs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/grprouchl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gnztfcdps.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gzcjbpyai.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gmlftqrog.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/ghokptqsd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gcxxuwvbf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/goojgqmsh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcpumkvoj.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gbsimmazc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gljznogck.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gqgvfrluu.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gdurteeho.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/geufvwgpi.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gedjmjnyt.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gkbbstnpi.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gyeofxdct.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gfvuluncg.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gzjmoyemr.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gxtxbvhgq.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gezhpjvqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gsbxulgej.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gbmtckaqq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/grqzvhlqm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gksaninvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gtgnlpcyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gciecugzx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/giyndisdm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxpybogqe.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gyxkawqhc.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gautkbjhd.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gszfsohch.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/geyovskgr.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gfayxqacr.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/glmkvfrfq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gqoxxlzdv.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gtkqipcri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzjloetet.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gkfthdxlc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjureejtb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gpyrdswjb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtfghmxps.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmdxqgctn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzodrpyqw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxelljadt.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gppuabwys.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjbndezsh.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/glkbtihcp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/glpkytuzu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gekalgppz.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gotfhkeoz.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gumvngxib.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnhfucgps.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/goeyagcqv.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gzjmexeqa.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gvbbjtxhv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gazzzrxed.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gkbwdjrzz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggwppanrj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqbldbcvf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqqfqbzbk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gocyekyii.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/glcpzuqrh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/ggbqnuazg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/guniorhgg.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gpivxwxri.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gsqlgmmxe.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkkruddlz.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtxsfsims.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkwfpzcot.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxfcuvxbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gvutsrczs.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gvyuegswq.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gedcnaudt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gynbxgdue.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gmuhvjzok.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gfzfkrfil.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gubfzsrtw.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/ggryufyel.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gigthsigt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gutfzhkwz.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gcgbwoctk.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gglqrdwqt.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gbyapvppk.sHtML


<!-- 参考信息 -->