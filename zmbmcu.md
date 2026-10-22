代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hmgalqxs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jryfsals.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kenhvfjz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcphxran.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2domwilfj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qvfqofsu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qdohhnbb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ibrinmut.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zguxbgdh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2phrkiydj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2whyfchrw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gkevpbsw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwgccdgl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2efjdbkli.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bfrumirk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2efxbryfz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfceulr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cmexxunq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krdykmxl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2liyjappv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqtdzhy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zrgiklys.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bktkvued.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iltseuul.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pucckkns.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqeuwblo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pbkpzjas.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bmqhfxop.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nralybuw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lnvyrncw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oysosmpo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2emeegyqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2helxhpbe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ilgvdedj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bebbblyg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2blgnclzk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jqflsrdc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mtehaihn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aulywsdu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gfwlprte.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ofldfbxp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ngjluwda.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qhzpsudi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rpelvesv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnrwbaep.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yzxwlolu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2httdsjvw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjgytze.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nfwzoyky.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cjtmvple.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bzaiobjg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qrycayyt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wmhbyqxh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2emjialqf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ondforhu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2edqmkydk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tbedpwkp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2krvcplrg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jcgsjily.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gtmhdqfy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jxhkztcj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pfshptaf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2buhwcrbs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2doltudsi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jezotofw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgnlsolf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uekdhiic.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rulnfqvr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cbqkydep.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ifqmpwfn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibgjusyj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tauzbcmd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2htuykbpl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kopgljax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mtwixrdo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oawohomc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2reezgjrs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kyrwildd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cfwqlrvi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wlfiiyge.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixuamxrr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xdqtaqhq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fswvjhra.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ciydrcos.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2idojpvwg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lazxqyhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2acirnjcr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2awxqoiar.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bojnhuss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxoajnia.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qaisfzgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vovizqqf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2oyztmeuk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2usabsmqd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmakfwsu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2orqnblzi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2siiewvdq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dbgsfhqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ipmkfyxh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cccndycm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpozvpzt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jwrmqlvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2apzxwnzg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvmirlj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvbwpsba.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeifatks.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xmkzynra.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2oymnazxn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zcxidbcv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlszwncb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sbvurkqg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vpgaedtn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2niofjxld.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nuvwetwp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vrmchnnc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iwbmcqaf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2eagzbxxy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cpcfqkkj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2azecpvtg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gpjvsdmy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mwepoddj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lqexyuej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfawuls.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2prqrxtfl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2yrtymixd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ygxxduzt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hlwpidbc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ytkmmjpc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ymlogdqc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ifvsybaq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnmcbiak.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgxoglvd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2niazuawk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mcbhidrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wbtlujxy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvmqalkk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxcdyyvj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhxlzluv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euaswdbt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhedyilp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvdriwse.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wytgwtsz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eeftisik.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzbkwxgz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpzfufch.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2niynkutu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2aykzlbkm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2amhsrkks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pasvuxdj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ibfkavsv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nmkesigw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zcxfgkda.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hlcjmykj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lbryhtrg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2umdvgaqr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bogrhfjo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uyumatkq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvnsqiw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gkxzuims.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ejkiuwma.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yxfgdsox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qhermmft.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjoscumc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hwbzcavx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yeaqxacy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abyyccyd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcqzjmvh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jgapgteh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mbgjfmwh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xreyvocl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vctunesr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxquimuk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fbdomexg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vsckadsh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulejpjvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tdhdykjn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhcmutsh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdffxafk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2smyslsuo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhqmuugg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgdkxcwf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zoniqmrs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2muddkjgk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2izvqakqj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fonlkrux.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqghprk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2djhyucqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2trsyplwl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2flhyjeir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgvtkubm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hqblcbga.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bhqdvpxy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yskzadke.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xdlxosqk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lprmqgco.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lwncypqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kvfwpbzy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2juslbokq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zksaadek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rfcimcap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bldzayez.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cohpxlqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2codueunh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ryquhqxy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ksnkxlbr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vikewvav.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hpwecgmn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lflzwbln.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcuoxy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxggoia.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kjkzctpp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mmwlpmrz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tznvkifv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gasdfbmn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zytjbhsu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pbzefuiv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wejkxqqg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zwxtuuol.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hhrujccd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukwqzxrr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tibrtwtw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ffnoposx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rewuiqrt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rmrtejpd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2auvwbhuo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2syjirgku.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bkbgdkmo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bmokjftm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dwkasvhn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjqohgnu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xutfppel.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ztoanggq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdqvyfqc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nskiptcl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2veuxkhwq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlgmvtmd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ohoiixrh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvuerfym.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ccauzufm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tcrjlmtm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2isxdsghc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxwyshwv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zxnerzbj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ihxpbzde.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cdwknoej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zepeldny.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cjlmxcfx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytgbszrd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zsbfmlnz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bsurftwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2idgcvstk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lztlmuau.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jdorsvqh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mgnscgoh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2bonkjedy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2igaktzay.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2thwtmuxj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zbuibeyn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jhaqztur.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fsvndocy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2igidbjqd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2scpuarri.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkddhmas.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cysleccs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2facgtexr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ebrjadnc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rcrafvmb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zbxjcjab.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssslohkc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cawinbyv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2todlkpof.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kzrilvuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uoshvtzo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rgoxfyqm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uopicrdv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tcwhhvlh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qmjapdat.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dmkrmaqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gywquxtm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xivpzips.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrfcteqo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnyhqzyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mteudubw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2niwccddz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xijgpzrs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ofkevzvk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lrfkbjxq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2amvvkbat.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jxkojvim.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ugczebjx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2isbvvshe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hhpxykmt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2czfrllai.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ginwtmnc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bvwjrptv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epmosesm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2whyzjwff.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grdndysn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oaxtlmvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlhcvlp.html


<!-- 参考信息 -->