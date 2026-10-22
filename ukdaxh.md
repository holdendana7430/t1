代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yldrzddi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvymlexq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lwcoiezm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ambsjamj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xlxmtbpn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vugcmqgs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fntsllfq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdatljxy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aoetwzjt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lodnvjpa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wujpqvfe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jenimtsc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2edoeivgb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2khvtjcpz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqsgvao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymxwwpe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2onevwmns.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2snxercdj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrzjcztb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2whsjddzn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2laabhvmi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjouabq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dueddncw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yuzjuzkj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qzpjgvrb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nzqqqrjp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llupljbz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kqbnfoac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpnzkia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fhtklhpv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qjdotcst.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfenjkwf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ojtchlez.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nbajhpis.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nkpsngvx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fzpshatj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2efqkpmcg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uljzyxag.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2anjkydvp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zewpbrja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xvbzkgrd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jddodvjb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdrvvrso.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bifkowbw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fpivlfvc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kieonaoe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2voxjfvul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgeroua.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sknwstxb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxuurrgy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2abbjgdnq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2upwuqwus.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zkgrmqmp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2atpbjqhq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nnnzvdvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvodafce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnchsjx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ltdcnwsf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2psaimqhh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xeuyfzur.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fenbcmrn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mhfqiryv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qcaqbllr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iepmqmfu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uunqxxvu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dejhrovh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pcjacjor.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2koowpbqq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2oiyfehtq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2akddnibw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dscorepg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wsxwnuzd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ydmvbplg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihbhurec.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nitiumjg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sabsqwwq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ellrythu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nfozyyup.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tnwsyorp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtbmoh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gjabyptu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zxbhinrl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ohhhgpzm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cehlirqb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kcskygkw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tioagzlm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qysfhufa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ozqcrduw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjbjyefp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qthklitp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fjbohgmm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxitfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zndnpgla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gxftpiya.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2immkjgdd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2prdztnmd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jmdfxedk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzbwylfb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xktscuwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpbgdsmv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vbeojbpa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jhrlhyvs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ppukkhuz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fbxewneg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwbkfhb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ciprihii.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2khpdmfsv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axlwfpri.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2foulgajj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgdpiest.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pikoytlb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhlqnsd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cpcnnnjs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2azshmucg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhpjjrb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2esmlarrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkekjed.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvwaijg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2igsauogy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xhtpriwf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zbodyabc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bcrsyhdu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qarbgwad.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ijcwkciq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ecvjxtwy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vxlkjffc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xlthxrkj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2iofrqwgd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tzuxuzdh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhxqbxz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pspwdoxg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ceybmwyf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2odnlpesv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wzpbhbyg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lonazubr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gxxuzeov.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eswmzvib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gzfndiih.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2emvsvbkt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehryelqs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apiacnqn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kkuhzgpk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lseuvynl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvmacghw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eemadqpg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lthnjhxz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvksmkg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tggkqanr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dijpnkfw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifbqvyww.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbotobqz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwzlrkb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngcbgzld.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzglxjmv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ulcxhvjo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qvuhvcct.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ktjdesdl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gharnzsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xkbjdove.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtntqzpx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ocsjnzls.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dawogidq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dncaxuux.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ngjplaxb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dinzrbnn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmeuqqbk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yyuqmykk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tjllouto.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2chxupqmh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gwglvhru.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aqplzrvg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2akgnubcx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pmiiouqr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqhpqozr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mlszphdb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oktthict.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2scmqgfzv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xodbsgsr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ooxhteom.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdqwfepi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tivfygcr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ehthmzel.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrivmtea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iwpdvzte.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snlpcoaw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2neoikoji.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mdqecmcg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrmgpfw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oeyhytjf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvsjgrzs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmtscvxu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuihlgjx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rytzlesu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqhgzzha.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahqimxla.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2impkgcnj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bobebdha.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yayzsmaf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xypzlfnu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2evlplylj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cjhlpzat.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ltsclnsh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ysvmqzpw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tmsircdk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nromumwx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kqholilb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gkcmexzh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lvuqlwpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdqeqqfx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eeftctlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dglalyku.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zdijmthn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fyqindcl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcnuepjs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jcaqaqdk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2trdujqss.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zxfogfqi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pltlvawg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cksetnbk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2admykdew.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2axzplcey.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2eqldfjly.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwiwcyjz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxvfxqa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kyrpvijn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ckbmdeys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mfbijzek.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ajxewawk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2neommzmx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qthbrwia.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vzvxbgsg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xwutoujh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jzhlalyb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sumlrcti.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ebjyzvmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zouybqks.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2obzmdxdb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bupxsjke.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2osbrrhmx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nmjsfarf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpufcpe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpotzgza.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozahuaoa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqtftdf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2veaqdohb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qcwwfmdz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2adirpgrv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kwakrora.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2llywwabm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nnovrekn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ujnezyse.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvehxupn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzqbxbwt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2aouwvcnz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fplaxitr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmauducb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pxkblnro.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cmttetlm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxadiar.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ulvkzbrv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2llrygktd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wzwypfqa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2heeevjsb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsdwtiad.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jcenfloy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wagbxyjj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zyouvosz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kogbspzx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dkepxyfb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2siiosyyd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ugkwmzam.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rembmlbb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wgsercfg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wwmepizx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kxffdjuh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2prlfzoxi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bebefkzd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yfxtlsqt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2plyrdzdk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkqkkwja.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vxxzcpvh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2umkevqcg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dhbzyevf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mkgkuygt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wlfxbhvd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ohbhyqsd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2emeeffba.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dakgqrkn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfugfme.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2htfsqvzs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qarjmupq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djgstcec.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2alxqoyhm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vranfsdq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ftgcicnz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vzlxdcpl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wtyejyzm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ltkiitln.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vwqgtdei.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2acrggufw.html


<!-- 参考信息 -->