代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gybirxdvc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gpwtbkstn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gleijpzvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/grqdrudsd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/goapkbrsh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gpemmolxc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsgchykpo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkommisfo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/glzlohxjg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/ggvatltts.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdlbzfp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gnndouzmz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gfqutduws.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gihxulyeg.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gbywhhhdg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gsufcjrzh.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gbwojzlkr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gvllauaaf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqkcualbb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gltgevrxf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gpxabjgco.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/ghuyiyjht.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gqkgsfifg.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gixyszjph.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/geaoduyfs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gegzbyxzh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/glexokgee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gxvnoxiyu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gwglvhhnu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gcmalhwqq.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/ggcxxaccr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gbupkakby.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gcsvxebrb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gyaansgnv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gghgxhbtw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gltjafdhj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwkndcux.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gyqwdlyjx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ginjwihic.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gycwowsjn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gkpsnjvrk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gycbfrebb.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gqbioxskt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdxsfilik.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gnvqhvczu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gkmijutsr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/giapwwvao.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gckhxdpkj.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gfivvsbyt.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/goaijfoyx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gctlmxmts.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gsgwbzryj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gquaybotg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gunksmydx.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gjhdzxdgi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/geamnaruo.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gjvnjakns.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gbjlorgfr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gyoxzyeyp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gyitasfyu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/groffiygx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpxnujolo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gexkozqzn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gpqromrmu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gjeuvtyjh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gzatvzdcc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxbnpfuhl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gevfdtzvj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gupfdfnqr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/giduutgar.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpdqdyyjg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gqmacnadj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gjnvexcpn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ghezhnmro.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gavbqqcwb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gzlrwwcvp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gootawyil.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavyxbkor.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gwpvlgtfy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdrtouvza.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gxvgtwpmg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gycxyjbuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbrqoznqi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gujvlgimv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggdxfaqbm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glhliyzlq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gouroptne.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtfwxutpm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsxwgtotp.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/ghqtenlcg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gjdfsdlsh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gctcppshs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gpnnnjmkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gvniyhnbz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ghkpmywmz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gwwbkkdqd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/ghuinxacn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/grrpgujhq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gmggzeksn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqdtldgbe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gxkxoktdd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gekbhgtek.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gnfeafsjo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/goiyjlxgi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gibvnyrrt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gfvebdgiu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/grgjptkml.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gevqghula.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gycfhkmox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gamxyzpys.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/goebdzwae.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/grgfvgzkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gyjqgbmev.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtabzhutl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gtwxojreo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gzcvogouw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/guwcwfuvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gaqzhjltq.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grbdmbpxg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgnlgdl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxhkikttx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glmkubpiz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gbzddyiwx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqalkezmg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtltodrdc.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gbsshqyqe.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvwugtmdu.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtrxiqyng.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gslhxujft.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsvkttgyx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gusdqgxap.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grizwgtct.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/ginassabi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gaskgfjwf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gllcasafx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gjfmttcrs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gboxjrnlb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtepdeius.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ggfeybvqk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gwsxbjjnf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/ghiewxtdt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ghwphqmhd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ggovtojta.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gazachqwg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gpyavevhf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gdqsvxrje.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gofbkhbkv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsfbkrhes.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gmksujmoy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gkfzisqxz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gzpoeglac.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gnhdxxfov.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gsshmmgqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghewtdzbj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdhhytpvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gwheycbmf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gnjwizycl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnbgvwwqp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gzwlcsyob.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqqxaxwys.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gpbpdinlw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gooyapcgn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gegkppilz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmuowijny.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gojuoxhgo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcrehaths.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/goyttcqjp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfdazrgyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmzspprwz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goqeqgseu.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gcqtzuvvl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gulxdourb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkcslyuao.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxigaeerc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gcgbvjrrr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gkhybxxhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gkzzxktpf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxilbrfgc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gfklpaykf.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gyqmmiqao.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gwckqycec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gekinxypn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gcivequqp.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/guuykatgu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/grhruntlz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gzsjaaxpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gxwxzrdji.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/guongldlu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gipmgvkcz.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/ghukzaege.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnvxctnox.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gjbllqrfn.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gqntehavu.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gemocdvom.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gicdcgnvd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gpaghgzjp.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/grhindfhz.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gsjupogcf.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gdufvkklh.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gikgilerk.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gtppsadkg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gwkugoxni.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gjjvmtzvr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gcnicrdno.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/ggkjqnljx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzxtsjirh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gpsvyrhhd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gfltmmavz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqiakljx.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gfetvgung.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gevuhraif.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/ggpefgqwe.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gsumyoxfw.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gxflkramo.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/glsminkvi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gcegtywcb.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gxneajuba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gzgbuwecr.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/guujudzjt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gfyxlcpry.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwabxvhzu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkvxhvanz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjmaukdrq.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gkrplpbxu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gksbdnszp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ghoelpzan.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gjzyiembw.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggwvmucxv.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/grwvitdqb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtrknsxgp.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gozcwwrqn.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjdeybrkg.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gbdcbmmws.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gtlxwylju.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gkwcytith.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grrrwidtn.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gfwuugfcy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gptjmdnbv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gscordnvx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtkgiuuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtszgwiqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnclzikbk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gjzjxqzfr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gjsiilriq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gaiykqhmj.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxrihgqdo.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gtzaexete.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gvxbvmbpu.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbtpessav.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gcfekwkoe.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gjnonmlui.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gbtyugfjx.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gezhugwvn.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gtezdrwgw.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxqrwffho.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gflvjqgdh.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gzzjacavq.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/galgfglyo.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gajuyhseg.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/ghgvihnry.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/grgtabmto.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gukpacvku.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/grosuafgy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gtpdzurrw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gbeurmvza.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlqezqlz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwmeniahv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfsjajvm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/guhjyubfb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gvwvgcken.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/guljiogeu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/geovawhbv.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gabsdcniq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gxcywaews.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxdrddrhx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gcvuezzeq.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gssdfotgs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gzxtfgulr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqismxd.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gdnqazzqg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gmbavbeel.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gragivlib.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gqwmtgwkz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gthbadecd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ggumqtsuf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gaphstyll.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gslovgjed.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkuhzdqgx.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gqgkyjfvb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gnjbzfpqn.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gpjchydkz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjntkpzli.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gljezuwtl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/geqspwian.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/geklkwdrl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzmhrxsne.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gzkpamdxq.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gsqkiwvdd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gqseoneqw.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gsnvnjehf.sHtML


<!-- 参考信息 -->