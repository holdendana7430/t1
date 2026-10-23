代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sqakemde.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jfouxpbi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yhnglolq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hfrffvrd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ajijmktl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vkqhhgrj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3owuvqkhq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ulquptoq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yzpusyza.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3epbwpscl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3maujpazr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vqafcyjd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3oxuaahpi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zbkhqspv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3edecgqqf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dnebwswk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3usnmqnkq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvpkkct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bzwbpuvq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qqijsxct.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iytowayy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lyvljhda.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tstyrodu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bzzbplaq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oqelbcbn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eslepsvr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uquwslsg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfpudiu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zjsnixmh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnrtzarx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkhqsy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qdvxomkr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rmvjzgaf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rfyfhrwf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3idxtpuaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyatrab.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ltipudsd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yffrmroh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tgcywfgp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nuftvgdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3cwmsajcd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3whpbbxdp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtbnpux.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oiiforgs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3avrjbcde.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hrgklepv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kgffsfji.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dmyqwciy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vbivxmwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pwlckgdx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ejamdrfp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfwwvtk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jeetrkbd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dioikhui.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmknamd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qisqfdxq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifkdvuou.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vnrxomgc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jywzrbkh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wyxvczoj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wysrixdt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eqlngxjy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iggnkkzj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yvwiylsq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ugrbxzrx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xtibtfhb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ehvkredn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gbteanol.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zfqjrhdq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tierpvnc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3thanbwme.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rrqtrnqq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzuystid.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ugigxlho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrgrjsnq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ndfzvrzb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cepeidrq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fwnuriic.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nrwzabwp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fmhltzbk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtjfzdwg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ohlmdeaa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jnxnamoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aydvtisp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gbsbstsp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3leuagdnp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tumkaijn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3djwzljhi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3itwbubgt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hqnfipik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3exkrhjdj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tumidsvf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3clykgehk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihatxpzr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pxfiutwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgifvgih.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uabnmuyn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3khulnwgg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bykcrglq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tqntbemu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bvkfnlvk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcvcgnff.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ynewrsrk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmjudpo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhuikpcn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahozlcvx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3grkrozox.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ysloievs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldeiccyc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gjmwmncz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fyksqthb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hizckbga.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rwyzvkhh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvdqbnl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tlsceoyb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rauxmgfh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pzdsycdu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xjtmjtwq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zvsprnvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgbmesn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzcftqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3omsrvlfs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3skxvssym.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ujmkkobt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ztkfixly.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gblbsuyk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqhqhxmo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rtlcztde.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gpxcdine.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qniymnsu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvmlcel.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3prkupljf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cconatyx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mgwpcrwk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adhizxjh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcugkfvr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntpadaeh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pftsjfkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3aesgifkb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbkjatud.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrzyzflj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mvmzpskq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryesyiwo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3enapcuvg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecospgux.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nweslalr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjvjuwzv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3relthnoi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eocftkzf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uqglrdhg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ogqqqocl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rziootav.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ampwiuhf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxlldqwa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3amqasfnd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fzdbtgte.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ukojgtqj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gofdbucd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dlqkbhdf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nqkpxwhz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rdrxmcmb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3alxgdyqz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tfqulcwz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dfueenik.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lbbbvhhl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jtbwdbcg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxtywi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jrpunapm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sjmugbjp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvnpbkpd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyhtiwze.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gbnrrwgn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3drhbpodh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kamrqgfb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uhebmgjc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azpgwhvr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lrmnzuxy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3unwdbeep.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3malothsz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tldbrhtt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yltjnhyv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrdyeowy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rddiaccj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bckkfldi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zekbzszs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihpxhkrn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mkzgutjg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyprsebo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhixycip.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfdytacs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vctxfevk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iyhfbgya.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hhtzbzkb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyafkjew.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dwlwpddx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fobcdvzw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3irtflqwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jqzftrkn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dnazbsay.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xoggawyy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gceftxnd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mjomrqun.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3frjmagte.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3onevemzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egnkhzfn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kcaaqpxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svtjlkjn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3iudmbbqe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rdwizbsk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yasmdtbd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3effzrnvn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngipuuib.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3owcszdav.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lehcilyv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rghlnbmy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbjeudvw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3smhsmlil.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3thgrbfht.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxrafmau.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rzssqoqw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3otiahnbk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euxgnyjh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jhvmnkmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3iyrcgtys.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esjpmmfj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbilxu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ycafsdce.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3skanpssv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ntqngmfb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3buvdihui.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hnzhexgz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hgokjkgn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bdttfapg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vtuhrzxg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3huebddcu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ullnbmwl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvvsdgzc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3demtytkq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xfbhiamb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fripftcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtiwcdp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lemeddvu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wucmwzso.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ojggtexw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3comhbyln.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iogvohjm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcaxdkyl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qbcgodji.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3erjqfojr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cjetxaqd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbbqkukz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztxcewlv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mehfvdvz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lfofwvpu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jdbrazzs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gchqgoqu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjjnsaum.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spknywxw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tbbxujfg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozhwpmkc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kwuhzqzz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kxeojygd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vvhkzsli.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hkofwxcp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewxhqcys.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bpamaall.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jtckrnza.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3llqikjrh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vkgkydpb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3plttarlb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qeowhned.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3duhfgrfy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nawcepas.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtkcakgb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvhffkrt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uuhmzjnm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nmmwngac.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzblulxh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3javvghwd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vcctforc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kmibenan.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvycfxeu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3sxjjfael.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqelddbh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3foosfqsr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gyxjpatp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bgvkktim.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3btseyxlv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zpyhfxap.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ecpchock.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oixofccs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tlckmwsz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jtffbkhu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wmqgaebk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3szirpvua.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lqtxcvxg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zluoekzm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3oudihrzp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zxpzgdgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3roymvfup.html


<!-- 参考信息 -->