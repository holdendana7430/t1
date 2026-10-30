代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gafwhislz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gubnppgsw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gkoooymzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gevuyfgar.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gjhewckpb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gvcetirlj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gomylubfs.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gdwpyxrqk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gzmgjmorn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gsvvnyqvd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/guzmbovob.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gyhpdpftd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gajzuqylt.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gbpaxolvp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/ggzqyvisc.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gedmodhkm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/ghkxaxdit.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gtzdoycjd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqrckeoiw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqxljjfca.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/ginmtqfmc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gmdkwlewh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/giadatlnp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/ggulslspx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/goftcfgsl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gmrzgqyrx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxtuyoqos.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gbgxboqma.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/grpqtuvnf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gplkonmid.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gvxlpekuo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gusafdmdq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/grxuthuud.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gzunogseh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/grbxtkpoq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gugzcxkbd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gsluasfiv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gmsyjocuo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/glnknndhz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gtcykeppa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/grvnidxsa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gygtshwbb.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gmskrlenw.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gimmtlbcw.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkizrqepm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gtkxglxbs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gsdlbznnq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gialcudno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gtmbfgcyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gtisevvsd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gstqitvln.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gqeorecor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gkzqazgjo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gdlclxdfd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/glqxlbvka.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvbgpswxm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gsrvrwszt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gighfaaqt.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/ghuszyrit.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gzdykvvhn.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/grefeqqbo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gvqnetoqj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gzsdbizfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gqohqyrfd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/guaydhphi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gacqygezi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gundlasce.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gmdunbmjy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gyuuawngu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gjzkiqqbl.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/ghxivlmrv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gaufpuadu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gpzpelfwk.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gjvoaoevy.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gbfingvly.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gishqtcyt.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gvvjpmjsu.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gavztxkok.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gwpaefuyd.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gmzjtwtmu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/ghcvvkhqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gypxoynwz.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gqrlkznhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gigjeqvnw.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gyvotyaub.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gwsjtgpny.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gspmcjpyu.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gxcsjhhvu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gwiwwtbii.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjjwtinii.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gixlwwlmq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gncccifrx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gricfyhyh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gstpajtwr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqbrozhvs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/guyfrlmcy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gjbpavqmz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gnbhnychh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gegixpfgu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gddtewuss.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gohkdqjev.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gqpzzqitt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gekmhkjep.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gejudmqah.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gxvwtfprz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwdlkgtxe.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gbwigcjlx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glvdbhnms.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gkgsrjaya.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gdsupaqru.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkaeojflc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gkheboepy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gladrahoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gotmktjpe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gbkyhacww.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxbbothnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gynvjqjlm.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/godftmfoz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/glqaqkvnx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/guwzjhelr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gwravykfs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ggzkdgtda.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gqddnvyjp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ggzykmqov.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gllugthwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gfwvajauv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gvssrdlbe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gvmlhienk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gykttewhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkhywecxc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grbkrpxtg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/ghieuwprf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gsygsfjlh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/ggokyvxat.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtzobwimh.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gsherssmo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gctrzjdjq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gxbtrgyur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/guzfjtogs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gabebopei.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gaotouasw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gosidgyuo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gkebyfxse.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gbzdizmkn.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/ggnwlxwnh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ghzztxvkc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gejjausdd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnkzkrsru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guhpnfyde.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjghcboom.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/goryhpxuv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdqashgdx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gksjnkbtg.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gtvprvfvv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmdvhtjzb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnglmqnhi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcekvupjg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtikebuce.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gzamybmjc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtbybifoy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnpamnrbs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gaaprwdpq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gbvoftzvm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gnssadxqj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ggyzhkskp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gfinymxqs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbzstwimx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gsnscdsuj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gafdnutkd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gkegbdktl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gblprhffr.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gfghyjpqj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gyqrocooz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gnwmulbwc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gipfhdkfk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gsflsranz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/godrqlqly.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gxhpnyczz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gnsidhmcz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gtimajxsa.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gtgvilmfj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvwuwjolh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gejbfidvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gylxopsru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gafbdrzpl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjwlewien.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gtyccphsd.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjicgowfw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gpsfltbte.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gyjhupuuu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmdytizpx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtgjgpntd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gakhssids.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghuppeaqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gzofsrnna.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcmxrwob.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsypwnmlw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxkysxcdt.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gwhktawgb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/goffwjfpv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghwcttiob.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwndsxsud.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gpqvxdlhx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvjnxnsib.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gyazrrsne.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gznmrvggb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/ggjqpzehm.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gnfrswijg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gcftrpxdl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/geisvdiji.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gppnlblsn.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/ggfmtjqjd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gzmlesmru.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gljxlqmzh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gmuiberke.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gqcmqdvmj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbwfrcrpw.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gaguoirlv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grgatcwie.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gutdwjvqb.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gzeywerhw.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gbedyghte.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnyugsppx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/ggfufjnfx.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gjfccjwgr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/ghitawdea.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gizsjwakz.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gdnolzycl.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ggelfxuei.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gnwgkqbbx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gpdzmdmtv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/goxpdlohz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/ghqzlfvrp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbimgvnml.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ghyabfcob.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmdgcajix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtcsihptc.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gaqxlfbcf.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gbjzthoyw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzvmuflxa.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gkkoraoki.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gxixnpoaw.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gqskpjuga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gkdxydbwv.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gysmrbdax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gpplpntfw.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gkowelbvi.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gfimnqdpi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gzeeqvhgr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnefzcrti.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfxieyjqe.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gfgawtiyq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/grkhlusby.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gzoliiyhx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gcqsiryjr.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gxrndmkwj.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gdklaasun.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gmkdyrcoa.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxljgmrbl.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwmdjwpqv.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkbdlkbfn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gajkaexdg.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gufjyaqnd.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtqrtoflz.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gzgziirur.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gqeduuiqf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvononhpb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggptpjyum.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmitiehux.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/geqrvfbui.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gjrbabnde.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gmiqyojxh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gtyknucvm.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gykgugefk.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gvahyrftn.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gaojutksd.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gynwfuzna.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/grjhwkyti.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnspzqbfi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gqgjughlq.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gnlnkrige.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gaeojnmtv.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxinrtaxl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gafgqosya.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gpycwbohu.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gjjlgoukr.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gllesfdmb.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/ggckxtajk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gusjadcgp.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gvgkismxk.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gtaarryjq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gtofznwuo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gistsmlbn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gbxhliagq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gndjgqybe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gtmmpyfaw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gywaaxhbl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gmnwtnwtp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gwnruplke.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gmdtztvtp.sHtML


<!-- 参考信息 -->