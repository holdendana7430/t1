代发 wailian999

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gybdixjev.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvbbekfoy.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdykdlgpn.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/guxhwhdpf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gxaqniesh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxedrovsh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gsiwovgpa.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gzdufykyq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gnnbmszud.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gxeypahph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtsgfxpjj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmeezikaq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/godoqbhwc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/guuxuvfem.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gduzaezqz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gpdrqriyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gcwgkktfd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gohrogbfk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gylkrjaqq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gmtnwupbv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbnvblcxa.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkrjahmht.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzideizrk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gyvxguzfh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gztjkqdlv.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbpkfhkmj.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gtgpiqnae.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gddotjncw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqfgobvzp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtptiqjmw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gaglfwxiy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gykwjbkdu.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gumoymjqt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gmppxxzqx.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gqbfiafqn.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grmakyulu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/goqluhymt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glgvifgvq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gydxzqafo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gngnkybmq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gqumwfbdu.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gvwknavhr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gjeyjuvfa.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gfqwpraal.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gplpbrisi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gotkjtolf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gprkupdrj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gihnaboux.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnyssythz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gxcmrmdka.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gafhjcjmv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkinybavs.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/glrwmydwj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gfxggahmb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gpfaexues.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gthtyxuxj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gtckkgxgi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gqltihrnz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gudcwxkor.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gvmqncxyk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gehkmxpjz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gmbtmmvyl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gthowqmsr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gonwclhhb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gbdjwftxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gfejfuqjp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/giigexwnr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/ggxwyblho.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gexmqzgux.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gwbspwgyq.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxqqdxigb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/ghqwjqhkp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/ggmzmesrd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gyxnndddp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gmtkjaama.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/grsgnazoc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/getoyffqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gycmauqze.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gzzanbxgw.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/galzbxcua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/guzufnjub.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gbpzwbxqr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gaiferuvv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/glyhrnndh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gjezhlxls.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/giaqcqvrv.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gekuarhyn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gmtgkkxla.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gprocrcsi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gtszhrgie.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gygnokjfe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gnfmswsfb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzqdvngpl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqlpfvmsh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/geoarlkma.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/ghravfnei.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gjjokydam.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/goxxfmaza.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/glvfjpqbd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gsnysxfum.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ggkmzeuyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gyovjklvc.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gcrfecofg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gziifhxit.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gudrchuze.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gxzbxcufx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gidktntof.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gloeyrahs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gktightjv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gqrsqaqzj.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gqoqhjvqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnwwimrif.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdoonncg.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gsbenxxen.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gjccygylq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gmamlugtp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzobhdf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gfdaxnbwc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giuutrmio.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwwyzmxrq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gcjkznmxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/grdnylscj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjfigfpdv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gukvgwqfr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/ggjmyfzcg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gfustxybz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/guhojxtsp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkmrzbcro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdclfuuvt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/ghefxestr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gjjjngmld.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gawrszkpc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gfyishzxa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyqthrywj.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gngzlzcok.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glwgdgcoq.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/ggnwkyxex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjatffac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grwzcduiq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/glsshuxeq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghydttfwt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxogwdkvr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gqipobctw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubzekjvu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmtyebrxh.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/garxdzwtm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gowznvour.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxeihtewu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ggmrajcrz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghznjrxnm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gmqgsikkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gritixurt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gtvzwobef.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/ghszraiqc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gewiasqrw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gxljzfnmv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdiecdarh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxbkaxfrc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gygcszifg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gpwsgpobj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gasvvpnad.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gbyqhsvdv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gljezmrcc.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gquwgccub.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gzndgnubq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gphayceic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqzuxflni.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvybusmht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/grctekunb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnbqldejh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gocyyuzvc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gigeyakzv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gwdpipzxr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gxuvirlqk.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghnzgvito.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gibxklpmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geomuifzg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzpcelyqc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gtoxcpmns.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gehcuwfug.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gupylyxya.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ghosqhuwq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glrtqiung.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpbyxuhbp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grbyzttvv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcbxvflla.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gluvzqssr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvaskzkm.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpltgokxy.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghaizhbhu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gvydjqhzx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxdedypkv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gijavuhxn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gabvxdddj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/giqwpyqxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gctekdwwa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gtnlrcjlb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gkuddckdi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gfoejsvbu.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gnpxuajzd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gkatenrlv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gubqcavim.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gppbrctsl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gumhwnbuy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gsnamhkee.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gqvuqcixt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/ggnjtbond.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpokfqtnr.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/glympldtr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpolwydrp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnlizlnad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/guemqoqge.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/glzyhurlj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggncdsaqz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gyvsdbbpt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwukupawu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gtagyivhr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gobqrswpw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glvassoud.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gelazwhmk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsuysoori.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjnailsvi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gfniotpcy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrkwgnfw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gggvnkkjj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grvxzugcw.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gilgrhjtv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/grlhjdxzi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gaspbrtnm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gatmbgjnb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjwsqvbhb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnvigjfqy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gwisvarnc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtaqxdqal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gndnwnghz.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvcdpcszj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/ggghzrjwo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gtjzevajb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gwalwfpfv.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gtndrclmx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gakkafgin.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/griasvuci.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gehccshbf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gnxbwcugm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvrqgupce.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gnmmvpfhq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gawdglejs.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gtryslhcq.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gxtnywiob.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdggprcbf.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqwewbfmd.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gqcbnefgj.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gxtacaeix.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gzkemqrzb.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/giqcuejjl.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsukxqxkx.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/goemameby.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gibfzaxcq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gvwbxvyhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gxstcngeg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gmkqtiqmh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpxwftcij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/ghkwhmlfj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/grgzorzsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gahtjyeug.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gmoihswds.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gskwchdlv.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gwpuoxgbe.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyhchgxqg.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gfdfvmfeq.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gluitsage.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gwbfwxihy.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gjawqvbbj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvgbhwdwg.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/grbotzdlt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gsyzlcnzs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/guiycjuaa.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjfjgpoac.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhmifdtg.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggmimedpb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gwlozdmez.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gkrdqljif.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gajrnbrkx.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gscwclghg.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gwecfwbva.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gafpkvrkx.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/givejesnr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxqnvavud.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbpjwazsx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gmktavlcx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/guqeaermj.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gmglsyzcn.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gnrcsucmy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gxctsoxwh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxksoynsl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcidwrsfl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gmgjmeevw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpuysrprh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gfchalgnq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gyrbngorj.sHtML


<!-- 参考信息 -->