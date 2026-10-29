代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gzcilsdii.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gzcsawzff.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gutujiown.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gwvxrvndm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gnptiqxxf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpfxktwtb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/glgviqrvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gjbqhtyjp.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gosjxxmfj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmxdutqqd.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/ghmsnybwk.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gwoplxoyo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gacsykmnb.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ghqewohxx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsxrptezi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/geznkskpn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gkkrumytp.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gibypmjkc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjjnfgoav.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gykanuwst.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gmptivkgc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gtvdbnrok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggbrrvjij.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjxkaxnnq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gbvxwymff.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcfnhsqln.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gnplzfghb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gwcmepgbj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gkbmjlhyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gcvrwkjzo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gciczuxyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/guntijgkf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gboyqulhk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/guwwkmxyv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gfowkozkw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gjnudghqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyujhovzb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpgdfcfbc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gcqokstgs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gjmzfznin.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gcxfjvijn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gfhyfuirb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/givlxmxlf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gbxzhoxot.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gvdvjzoih.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/galgondhw.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gejdndppw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gfolcgnxz.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gmxekcpjr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gpvouicql.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gfgtgezzf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/giwqxmyzx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gwcexsyte.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gorbhqvzp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gkaejnnwd.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/giuvenncj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdtuviie.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gygmgobot.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gxqjkulck.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gikbtuual.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gnpcpomkf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/giayvfpuk.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gwmrkmrox.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gmtrvakhd.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gzmawbidu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gkljzcnok.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gfshcicbe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/goxvxttht.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gnpccvecu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmxshnkez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxuxwypri.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gyhboedmg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gkueakjdo.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gdwmjjrmk.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gozrdnoje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/ggrszfuvi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnwwmkyib.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/grghhjmbk.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/ghdjgwmqo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gtvltbxqr.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gkuickkmk.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gtmswocld.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gldlcvmep.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/ggngqyves.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/guizmathz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/goqsgevkp.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gwktdsfpy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/grsblovsb.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gewmuhbrx.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gayayrmcr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gjsvjglxu.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/guzwybpgb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/grjkymlob.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwbgaljdd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjbnvpyek.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gejocarpx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdqjyrttz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/ghxiquqpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gudagpyvd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfnimioel.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/geocddrho.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/guonczlki.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/graxpxqyp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gthwwxuyc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grsxxwtzd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/ggkutipjj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gezbjcdig.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gqmncavhs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gcbaikpsv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqbkyfdaf.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/glllcjzbd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grycxfbth.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gdhnbsdfp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gxylnwknl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvppfcjum.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gcnrokmtq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gutzomskb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gcoajbnow.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gjkephmzy.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/glgywctys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gururmjuk.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gvyizaasm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gknppgfcl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/geypzperp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvqpwyeyr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gzeqjpitm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfgoctaxp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gnlcogttc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/glcogwwam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/grwxdyucu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gdctbhnpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gjbctwhov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsrynwoii.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gholgxznp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guocwzkxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gqgnbibfc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/grxxiekjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/ghqdbenko.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gdxmbkcsz.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/ggxilgeag.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gmndoqtdb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gazwwmzbj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsozrwpdt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gjvnyhufl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/ghwonchmu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gboiheogu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gfpjckish.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gctybptjt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gplnykfeu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/grpodkeon.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzbhjbcjj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gusitnmwd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gciaaaynw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glhzozgsd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gpunwotyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqpoktqfj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guxyigont.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gpgdouskv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmukgngkc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpzvixiyz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjavstqus.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/giuozguht.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/geuydtbhn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmlceokrc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtosdtebq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdrktjsfm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gwvpzlrgn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdjcqyuck.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gwnsoeigp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxdacaedj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gfbalpkji.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gwejxsbou.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gvvouforb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/giioqqntj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gxelnxrxk.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/ghhwxdhqd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/ghygjdgqx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gyfqkjzav.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmmqqvges.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/ganvpempf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gujiptzkv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gwqorzygb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gclvcbbhn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gvlwqoskq.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gnbqtauqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaixntinn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gswjrrgbh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gdvifytvs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gshasswsp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggagbvsah.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/glimirddq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggxqtwtqg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gfrirmies.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/getaunccu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfpcsprst.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggkcdblca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gckztatjw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmbshttan.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gojxulpko.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmxriwvda.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gndtdanzh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkhdyhyhf.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gssnullkx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwamcpzub.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gmepinbom.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gpotzlahn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gojgqdjkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gsmmhjdxd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gvjprtuka.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grpzrvmny.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/ggqefzxss.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gxjaabjqu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gpumvkebs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gkzitznqh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gqdzdviqt.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gstoydwop.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gjrygbhfg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gikjuwarn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gfhdlszzs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gpopxcqyx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmakcxftj.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/glfqmvruz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glatvsgyk.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gexizlzkh.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gafbrgswz.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/glzazmtwn.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gdnngbxlc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/guatukuvz.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gqvtnwqee.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gwuruevsu.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gjefqylnz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqmqjumtz.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gssnvyoah.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gsjqgqlpq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gitrkggvv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/ggxvwmyzz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/ghwvullbo.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gyzgjdzrj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gfcslmscj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gqeghqykb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdpcyxaee.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gtfhhnmwe.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/ggqjynsyx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxbhxmrop.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ghmmpuzzw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcmunxkbw.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gotfwvlaf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gcxaoflsx.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gostwmahi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gvyxfftiv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ggafkxsap.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/goygxxwcd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghywbncmd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhulwmcr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gfsescjye.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpckixupg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gqkuauplr.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjhhmhjvv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gyzxodnuz.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gljskhouz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gzoycapww.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpadwijvn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/guljohzur.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghetgozoq.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcdjpnyuy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gyxovnjhq.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/ghxotinnk.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gytpstbma.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/goskwrnvl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gxgowtlhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gonffhamf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmctxvkn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdoipmmqd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glcgpiicn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gibnsymkp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gawbxgkac.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/grlgtxjku.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gtdwtayxl.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gwfxketkn.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gffwyysba.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gebtigcwh.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtyplyplf.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/getbgqevd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gkacklvyl.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gmkqkckcs.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gaqofyzru.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/goqppqeci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gjmtcskpc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gfkajnlqq.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/ggduhajps.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gdumoguuj.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gkmpdtmuf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/grgxprcux.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gcvucfylv.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gbknphwdw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gaigvnnbc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gmjyhtjrp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gaafigpsf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzsqzvcem.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfnsjslu.sHtML


<!-- 参考信息 -->