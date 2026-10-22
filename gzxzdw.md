代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eqhebidd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sokqemen.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmeehxou.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aaebcbmi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vytdcdoj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2acgkswiq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tkfqjvst.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uohhiktk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eupdhcwy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aigtbmyd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vwnyrgon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2exdpfwla.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axgbnvpg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gbegzfqy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gmjnpivt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gixiyjwu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fiegyqpu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2aafvsklx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cdjfwtnj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2trcgpfnv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hekexlyc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rwkimkog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ywtwticj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlxwrup.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mlomjnso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ljqwluon.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vwednsul.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zldnaclf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xjizfvpl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rilizsew.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hbmkshty.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2askqknnu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ignekyfe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2szfqxptb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dupnutah.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pkbpimvq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kwqygake.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2loyatmhk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxfjrlv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jhxquxeg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbxjoln.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fendmobb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtlslyl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2bcljncfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iipjajnx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pdyrgqnp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2oyjsqrqv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2poznmwch.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wrdgoeag.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2crjjanpy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dmfjuslw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2oaielzao.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zxgqmsec.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gnxplnhi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dcdxhbhi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xaxtouwo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ldwugtzf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gzcnegkv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltczweys.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gsniwyww.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpymnkom.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dfsfwgkp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tnnpaxvx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2okbuoaeq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2huazqfny.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2isjusdoh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzmhwtfs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2quhkxuow.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqhidwuw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fjnuxtjb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nqqdavip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qidnofqe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ghncyagd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itionjwk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lvsuoqhd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lyuazvpv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gkomjjux.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mkscqmbb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yrllljce.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wrjysjdj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xolxjvbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcgdohfc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ikvkmndn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsmdastv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ndrtusdj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tdzmjnyf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gguxwsgf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lyoulsql.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2triqfbgp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuisvrfo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uazdhinf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsvuzcqw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdletcqi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rgyklqky.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ycwvzjtv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhcqijj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufiadbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vydmejty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qjqdkqzg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wnnxjgvl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dkfemfsc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlatsxvo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dosxkrto.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2abveqnnt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jyeghyjf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rsbgwdlu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yhzrupnx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uhuljigg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oebdldpf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qvlygdhd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rllwmang.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fepolalb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2enpbjyvq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kkriqjrn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xxbothei.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vzpklqcu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vjifzlom.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2heuxfboq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hopzspwe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fafhxjmj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xfzgqlvg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cbgnokqz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlifrmdk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhvdsdrg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axnizknz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2olphtkdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2huancant.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgzcbwoo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqscdalt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjavnali.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ruznmcjg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xausydnd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixhqlzxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbismopx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zmnhfjta.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvxhqkvq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbpmrfyo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivroirjn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gbtwmvef.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fhpcwdsu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iceonqcj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ypkxazjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tkfrmyzz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozrvdwfb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjfodeh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lmvtzsps.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eokvtmlu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jlxekaux.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hrnoaubo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjjaimvx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2onastwrh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nzbcbyqg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zmudpwjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khdcgtnc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fmgzgtrt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tkpvppuv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wvuvrfbk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgjcqxxn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2baajzmiq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mvtqzwuy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nijkfvhn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwjeybcn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2toarkwoh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmopclkm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ychjvliu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2osdmshvo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcfnrjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wdsyaqfu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoswlmlg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxksugk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qgvkzrum.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmhvefj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kutfynwc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2soiayuyo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2umdxxlqr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlzifsaw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozidqtcb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlglwso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynqzmhko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtxatvp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wfvazttr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2snpfpnwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hfhvtdyc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ppqzspcx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mpesrgue.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hppnclqj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zmhmkter.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ibgigrfe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2loyarsgk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2njrauftk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2esldnzgj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dxswqidq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpnyupbs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jbgcccyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kamcshmg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2apcpiicx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gbwtpgee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bjpphdfx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcsbetip.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2abstizgx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjxbes.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xozxfjer.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eplanbfa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kfomvfkp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2luawyomr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bhieutql.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mddtqdzt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oufpgtum.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcmrbbde.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jhruybbz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kweqfikc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yzgoutyy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwyvjlub.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eguyhtop.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bybxlzlp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jcbjsdjm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ijiwykbq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xdwdhypa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nnkumtjd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rnbqlneq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2myzvhhtp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kbodnndy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ugjtosuv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xukcyocu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fqqpgwvs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ezcwtidc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xsluvmnw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vlqsckxe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2upkkqill.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ktgouahi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zwxyhyrr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bgboysjz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jeoyjboz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jhnsxiyw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikysjzjm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cqcnjdcd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qecsjjse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rhzxpjsj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdjnrvbf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bkulzrta.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tajjjnfl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wpmgdvbt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvharlk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2obyoxzwf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxagbiqz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nazrpugx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tncxetie.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcgrdgcd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2smqkassn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vmscexdr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2feaafkyh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gtyyqayr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rxpbnewj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ykzquuzh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zpkhgylo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uwtpumxl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vzrrwkmc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2srnprjrn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylhvtxen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ryrknecm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2isbuczpz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqdmiapj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bsmmrmkq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjwarxfq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wrienzwm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lpubmwom.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dncuauaq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2onpjfzqr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nfxckvsk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rdrozuxl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2udofgcfz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dtxpidda.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nvymehko.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uzehnlnu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qzxgbtju.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stgutfai.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jnackwqb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zudwedsb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iqsqxwhw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ntxvqakg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mwcgyfvt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hiyjkwgg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zzsaaxpu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fvqmspry.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yzawrevz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sihlllpr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qppidmkk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krylvawk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mdpellit.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nkbvktir.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tldxjfnb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aeqlmbfw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2edpisiui.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lczhvizl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2njckhaoz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lnmdigeo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bwcdhibd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmqjyecs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2breqrhdo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xiwvilci.html


<!-- 参考信息 -->