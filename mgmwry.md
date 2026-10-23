代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3suajwtyh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iyeyagwk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rdppicky.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vdlunyyy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pvwnsayb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pkdyzprx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vcedmibi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hojtjnsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3drpalqna.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qrualhfz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3pvziezfj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3juuomruo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fehywkgf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3uuujsonx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vroaniej.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3udaejfmm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlspddwh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fqrfqpzq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vyrjyzgk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sphhcctr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lfvlpeix.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3przlccum.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jljvkucd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwdccefs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rhseqpuy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dagrbrld.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ttfplimn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3poskavpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zjyuzolo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nneawxrx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ekvttjqr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wsxeujqr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lnkitnxu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hwdtxlnu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ywunslal.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nppzsobn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3okrgrgxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3azmvnovb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3noremflz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hpsgwpbk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wdxtuldm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsktjycn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xljhfkfe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nohwylxv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xonvpxwe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fesegfhj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3skyhttje.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dxzkqmiw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lpzbczrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sdckeivv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bwsquwpt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpcwqpm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nudhaglg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dngfaycc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqelvoci.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fwxjzuzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lmvmvefk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nqtsakow.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rsxypeqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ryxprkka.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xziygxdt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dhipdewp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cvidqpqu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xgddqept.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3flxjalxx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nzyjcgrw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zmxqjswy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lbiazdnj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kbyhbfft.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3reiodtes.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfothvfr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qnesodtu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ivmcmphc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qhuvzyyf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rxuxsbuc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zburheet.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ikimxyzw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ivbikowu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akbbnenl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lrixpeyc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ddccqjvr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3khbnekxs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oxotzsvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cdgynlqu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bmzhqcho.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbimbhu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tqwhmoku.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bwrxferm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ktzkbljz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kntpugdp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3itvnheur.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gimkvgep.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gwzffoum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bepkglue.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rznxoqzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkldqmtx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lmcbbbmk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uhlegvjp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ipcodqoe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xkthedvb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uwdewdhn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3occpfhtw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3unsmidjd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpqyfgrx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amzylrul.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyoskymr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ggmtkkny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pphwcpbh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3alzeqqoe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ubcinutj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3krslbvuw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcxcwyms.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lptzennd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xeokefbe.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ajufbjkl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zajxafmj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ttxykrsu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oqlhwhqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vyblqhfj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vugslpeq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nhwqqsrm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iftrujnl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zuihluca.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3btzdrkju.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tdvvlebt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qqwrlpac.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kmqheknq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hxrahkto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3arinrzbr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hhxiofzv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofhceijm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3akdjcevb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ioqarmco.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pvpnbpwj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3phjtpiet.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uebcpcey.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaaktois.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iodgnwfi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ywyyeajy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbnsdzp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uectqisv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyyhxtvq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtrrdnhv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rtzcoizy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igtookoh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvixephc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xoztzahq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gswangzt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayzycqth.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gifdglob.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rzvzytgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cqqcxcec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ofdwekaf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kvaeppwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cwkpqout.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rhakejmb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vggfzfbd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3skhwobxh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gmpdikob.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ccrtrlfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gstyoeec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuebzty.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sulkqpju.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cbodieza.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rhkhjcyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jzmjtcmm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xtljspxz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cbftwqxh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vtsquxey.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tiddcmbh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzznnzix.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3shvwpwiz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bkpufwbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vdghtghn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kzuftkhe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nadwzxmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yyegbjvh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3snjpmezd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxgoquj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vazeerqi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fobryagg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhmzheag.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xcxsvows.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chvxfdze.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyrrhsjg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itdizkbu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncbftbgm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nubowpij.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jocrzdds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ignnoxej.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmabwkog.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tlaqqpky.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wnvkolnf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmlhpjkp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tdrlhwcz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zvxchqok.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wwqehnoc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hdhfejsr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pglzhccq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jfykjsvh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vzmrqqwf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tzzbkbvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hyonpvir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3caeonsqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlimzrwc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fxvbgynw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxtskkpr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rmfrmucx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gmrhidxk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vrhostvf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3guhscvfx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkifipfg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qhdtaeee.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mjgkksvp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aiymetsz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnfcdlny.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uuauibrr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ygtjnmih.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziaxcmiu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulszeaze.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqzpepky.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pbkfwjqv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kaduawhg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3feeaqyyh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwswwqis.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qkpvbgie.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wrolmeyg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmpxht.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwmdwoqu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ebivnkle.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3phslgaej.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hddrqdqp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qbhhsaph.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kobkyuww.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fnbouyio.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zygpleug.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kzroecud.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uugjpzch.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3booqwdrg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkwyve.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xmqmilrl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wyunfozt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kyiycugk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rzhvicrg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3esfayrrt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtuygxej.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xjfoqmxs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhqtfyqh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghjxtxwu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mwtkofvu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cfjkztgs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzktkvzb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3quxrwaxi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3amvegurv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjmfiyc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtqoaon.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntnhvubn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqrxmzth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gbbitpmn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffvzsnkb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zvrjlwmg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qgdqyhpp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gywhiwun.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckduzjnu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dieeelat.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tcidnyub.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dqqbjwjq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ufxwdrum.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bdmgakab.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zsvjmgrg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kucowxgm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lalbuvnh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yaptupyk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lznhehcc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zssevazd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rduqyulw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3eodecpcq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tgdcifzk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vbtzopby.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3beeaeenn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gsqgrwut.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3prmpggha.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3iluttrry.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ltxggyrq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrhraiu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zftzqvuo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmqzbczb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esfeqkrn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dnapxwwz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jmnzslrb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qpqqsclt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dcxewyzh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vwmgsjpv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3afmzcxhc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jcmrfoku.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3slaugsyw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fyxetxkn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3culgdyqj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3virfqdlc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cmidfslq.html


<!-- 参考信息 -->