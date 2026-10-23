代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zxnofsia.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mzrwuljz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkdaysna.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fahhduvu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmgphtvx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wsfoauhd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dkemfgav.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gvgteudi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bqqpmowl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rdldzwou.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kuqgkgjw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zqztnztk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wghxpkcn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3debscito.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3itniktyk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkdysxr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3txvykbnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kfnbwtbg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jjmvaluc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3knimgqvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hyawhjly.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ecyisdmi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gtjpfmmb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3momtnkkh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qqzcwmvk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xrblwmdn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xovtpxgj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfopjrgz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wuwmdzcv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ubeyvtcu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3scthoeep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sesmlrwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wqkfyvwy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jrqgaywu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uuupatot.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uhcazsjl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jgvmrkpg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ryhevfrs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xhovfbpy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3szqyatke.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ulmgcxzh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fdnmapdc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cljmtohx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3eqnswodw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vkejoezq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dcgxyoye.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3edsvgqbv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3njoiyylg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jckjmnqf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ivtviwio.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lzehujkw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wtxwtyet.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3byfszxcu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xgbdfxow.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qyfpfnjq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3luhpfepq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmlacsuo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxqxrsy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udqoxlfq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3izjyohhf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uwywxcmf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hpdjwrtf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mzsqeorm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3epjljdag.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eymtcwdt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxkcbvl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xvcldygu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3djhqrjhj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3sxfhpdmy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tlyjdwor.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nmtncbye.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ndlmtxyb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jxbonoms.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foomwvsh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lknzyqip.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rkaxxdei.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tynknlmh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rxgvsldf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3aoezksyn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lxqdehwx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tyjkdtqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rfpiqdli.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xfoohzpy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ngovatlc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lenckqjv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jrklbhea.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tlkfnfko.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nfiwlnbw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xoljlqkj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrnrkn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bmijfelk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aybrpkim.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hmpemcak.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qttsoibz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zsjlydxs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tuhmddet.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bnttdiom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efxdsugw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3obrlbnol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnxgsmqu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gxztccpc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ddvlatqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3figdycej.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3llgycoyi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yzituuyp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jaqnlybj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rncnjfst.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyyqknjg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tfzkskrs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3exfxuisa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3orjpppla.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsewtfyw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbtirajt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dwpcyucd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ygdmykpo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ftdtsoxu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3aadactsk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hnsszsbo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jecsueaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlmbsg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ftjiplgg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kzrekuzv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nxtaicpf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wfdfnryq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fouhuyio.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdphwgc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lltndiyn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mgbmggna.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oqgjmwio.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3turissct.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xvjdohtg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3klbfegmu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qzsdmqtr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3glzlnodo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zysmunew.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tklxsiog.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lvumvvoh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ybjcafrr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hpouyvau.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfmdwrxg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3diruoubr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eceflplk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wgsqrrih.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xslrhyqm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqnmnipx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ytkomndl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xglrjuwk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kgtupblo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylewnoqc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eafwuxkx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ajkpnxbo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewjdkaao.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcezguob.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zrcrerhn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xblomqqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbxtixwn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvncahii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3syzvibae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dsrhpzxt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3eqrlfzpy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mupkgvso.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cvramaas.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lpeyvyiq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hfivudmn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wsdbxqji.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaycjjrx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ekxmjxls.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nesuxxzt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzhkicf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jlsngeqb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjqktpnm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hdizxhtz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ryzygtcg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isymieyq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkbjhmpb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jyzploko.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3opifgihk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jvtmushx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bbkymrjr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkmbxucz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zlptcjbj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hymhhsot.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzxbrkcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fskpuqyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnzlryme.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfdenr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3glyrdxto.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aceaewsy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gngnzjrt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpamrgnj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlxtizho.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqhvawnn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wahywpxb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljezzaji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nalzespl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqrxpdy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nmxolwuv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twcwtxme.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3moxtbgcn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hrcxwwmj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsctese.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ypbgyrpi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kesbhksl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3anexrmgw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uliwotcw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mwgfhibf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bmqqstdz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3epzghoie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvuelvyg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ktuupqve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfwhnmwm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xrkeioyz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ajflxobe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3veuhjbmf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sxtlfbxh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvpcacu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bummwtci.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkovgjr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ompuzmzn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khrykkdo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ystdyxfx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nfqyurjw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zimtpbok.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxivhzyi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uiwsgezj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zmhtvqbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xdeowjsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jpggtyxv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dctocutl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3llwsixlr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3whkigowc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rzxxkfuf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yywoiwtg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gxtefkzb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xejskdep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3thlhtptk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jkkrvppu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hcvukaiz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hkrjcfdp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3brcczput.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wuzmbkyi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3akrgspxx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vilupgsw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iouwfbeb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cjnlaixx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqivhhyw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rljlkvyv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nhsvkwvp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dboupwon.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bbhpkbri.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfhoidjo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3chnzsztr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wfmazzpz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xotxvbpl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3khsfkgss.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rocclpog.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nclvjjtn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wthwcmmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdyhwuga.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cywemvyc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dnojsdie.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlanklxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yedspagh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mianvhnh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zwbgfwhy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3konnyqqe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3itpknwbm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cqphfcoi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hgicfkop.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zldppbvd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tugilvzh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wusturid.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3clddmehk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfyqdnuc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ojboindc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wedjzhok.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3crtzvepu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kswxerpu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmlrrqfq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ddscwvhx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fagoaxzx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nvrgelec.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cbydzfmd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3laayrggn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lywujyrp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwqsoz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nsgpyiuh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pdyakthw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eiotjntd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3astgtyll.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qmmokdsl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvfjepf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ktdzwlim.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fzzzdjdu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jqzcpphr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bdrwmnhc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3djfmnoqe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fagpcgme.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ytryftiv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kngdevwk.html


<!-- 参考信息 -->