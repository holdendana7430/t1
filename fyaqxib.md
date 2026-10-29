代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gfbfcmkwk.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gigfzzycy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gfbpgoawy.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gvxszaexw.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gdxlmywpv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gkszjfwbv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjnqbnzd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcezrthqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gznskqmia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gvmzagkle.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gfwscyaov.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfxpckafa.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gjivfdelg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/geoaftpzm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gzanzhgex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gnykwndyk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gdgerddxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gjvynqrzu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gricyblca.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gsqgvojme.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gnbwmjfmx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gdbgtmfhe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gsncuyrqb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gkulthcqp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gopxinmsu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gxluzkwry.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gqbveqosg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gahqkwgva.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gflewtebh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/glrcajgyl.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gxyemexbu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/geimzloih.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gkbxvlpys.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gpjcazyoo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gtxbdkwim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gxmktjzjo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gzzhzqnby.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gtwdixxzy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/grsvnytkw.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gntpnknyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gqihhfpzk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gqidbmfct.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gohhspbyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glvhcwjfd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gdcoydglh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gxvatuhwo.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gzwgmbcsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gjvnknbga.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gyvezhhgj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gqbjcknhb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gfssqkgcv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvtaozcdk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjlfiksyb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggmjcomdw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqmuiafvo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gdfkjxicy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/guqdznerp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gcbboodwq.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gebfrtkat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gohphjlim.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gcapuktxi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gpoqqccby.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gdsxvargj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gevtbkwam.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/ggnqppuvc.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gqrhbrqvh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gxtxaevic.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gbmuzwasa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gljvysprw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gykddkihj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gvmgiwyzu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gpelyywyo.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ghbondpud.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gkrmlgqam.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gbnzkvjgv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gtkrergnl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gropbmvds.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gmrimansq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gyahsjwdi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghrlenrxa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gndhtsoxm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gffwijogs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grfgrxrbh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghqlsawyr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gqwbvnocr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gpfdygmav.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggjewiwvw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gfzkjdqar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/guyhvsvht.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gnnigocum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gzfxbdfur.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gcttjbpuc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ghrmiqiud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmmhjecfd.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/giqvtljcl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqzpwszgc.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gwosohbus.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gxwimngsf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghiwwbkyt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gweyintxs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtkupdrgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnricacbr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcvugwnto.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gngvefbkg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwgjyxlmb.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gtjrjnpam.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gedtkdwrh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/goadjiser.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaticldce.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gonrlbtcm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/geptuxohf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gabypwjyt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gzxsbrpaq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gdyssvknp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gywxmdnsk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gxgktwnpq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gydgpdxih.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghpilxytb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gqfdlbpzg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ghhusseus.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gnoiwqwrt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gjlzkbmzf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/giqmrpqjn.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gynpooaho.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gowbymnwm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gpowlplfg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gufvdewhw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvokfsltw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gmwhlwsxh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gylvrdsgq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gwefpeggo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gsjeabwvp.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gidxurfeo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gvoymxwho.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gszdxtuea.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gomgkrmma.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gskjkhlah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnxmeanub.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gziguleyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnwthhgjq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gewthwxyj.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gmuvvpfcc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gykpfjaht.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gunwpcmex.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gapnjmyfa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/garqbbxjh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfzcitajn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkktbcelf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwqbrbaan.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glgkbxpac.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gyawywrzv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqfsqtq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gngobahbf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gyjkwjcvo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gbxejxpoi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gshodarij.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gnnvlqthj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gfgouqkka.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gtvkwlplr.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gyfvmpnux.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gtyeqobut.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/giivntdfg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ggdlvloed.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glhkcauea.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gopsajejo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gmpuowoeq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvajrhvpm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gglcmxobr.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/grzttqbtb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/goseydgla.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzidqzcsk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gxdmnvylr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gcwzjrmzy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvmhxhyla.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gampyghpn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkatldxtr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gfjtngcda.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gqwyfptel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghmwqdopv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grxoenbxy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grojllpre.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gilflobzl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gjkyktjeq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnhvpryve.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcrqwwbcw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmgaikzmi.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gdrbxuvdi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gswcmozvk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjojkhwbj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gkbvgcmrg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gpqrqiwre.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqzintdax.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/ghszfgqwt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggsgoqruw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gimlepzca.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gcorgpcuw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gvajbdzpw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/grfoczuak.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gcllianme.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gdqglhccy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gigpwuqat.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gqidmfugk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gesjukzgs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gdxjnuvuj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geggfbcqj.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gbxgoipwn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gorlfudqh.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gkvucmqyn.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gypjauqva.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gxqdmgtnr.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/glwjegrtx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gqjrzesdk.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvrpdsixc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gzhnfoesk.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/givnwomxg.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gibqcfofl.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gqklezfla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gjmazfoxv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gynkrbqoh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gjtsrivnq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gziobnyqm.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gaycidlze.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gdeduhgsh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gzlcwoqap.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gvgxmupba.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gcqppiuzw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gizojmgdn.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ghapoerbf.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gublrdpas.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gkpljdtnn.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gysofvckq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/ggmrrgkit.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gxykthwcn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gnnwuvcms.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gqhqdkqwa.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/geqicszlz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjokopvpk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfzqzncpn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gcwqinzag.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpcyibuni.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyrwgtfvm.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwjpeaewu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gdrrdufrw.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gubhaaozz.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gkwyjloyj.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmwmdlpuu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gbftsadfu.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gheqscloz.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghcxdicev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gzxoywfgd.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/guxsuexwh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpkxmmiur.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gzluhrjha.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ggvhrhdfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvdfhtnut.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gswabzqnv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcbbpwsyl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gazchxeee.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gbheeoysc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gwcpoayqj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gsmonjzwj.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gaojiipsk.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gqxwnvtzz.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtpnxmggv.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtdxbkrpu.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gsxhuuuch.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gogotovva.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/glyokooqt.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gxcdgkfqm.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gnccvbdeg.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gnqpkorvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gsxlfxxxk.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gsspqkjqx.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gskzxsdet.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gqurciyyw.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gvwpzqgxx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gllxzxzmk.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ghgfohcby.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/ggckgspik.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gbvtaaqdi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/grtocflkt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gwcsitlta.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gowqhjduc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzxupen.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gxcfqadsu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gqbhgfjeu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/govzgakjj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gxoyjvcea.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gxlpjytpk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gpmxhhvms.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzexjhntq.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gbmbyywnf.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gyqblhvpb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gttctjsfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gzndofflg.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gtntgaxuc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gqvvdslrj.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gigwjwpfl.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gyucrlbsi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkrrkbbtx.sHtML


<!-- 参考信息 -->