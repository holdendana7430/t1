代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hiyuhnjb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3thwkaxkg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojuuslnm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3brhciess.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zyomwcfd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3alijqtib.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ebvlmupt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hkmymqcv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3eifprpzo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xevhgcfk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fyqpcyzs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbwnmn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ztrmmuwj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpmheiln.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3eqgrnrsc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnykaiw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cdstylad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kknafjpf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cbiwuqsg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dnaysobh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qcjtrxzq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aoevagqk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vsanqbsi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3elerpotl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzyavto.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hxbjamrj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hthwscci.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kitpjpto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nvfhmbss.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3haffackp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cfufjwew.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3daicztkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3basiamgm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3swyjuclb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aitvyqrs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mbbqtooz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cibijxwy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3flihhoeb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zhdnhdjr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mbovkmfh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cmqlkqvh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sucimchi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ncgibmwa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bqmihphz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sgoosizf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gmybuxnb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aquafqny.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqqpawm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqporgsg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gugbiych.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tgnwhrzn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mkcqvizo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tmqowuwk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mbdjxqgp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qdmqcixy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulwipqjp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3awuehgvq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vqlfathz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfhhlya.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldyowipv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3njbdfcrc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ugabqlyh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3skkzsgfv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cquyddmk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aftvqjfm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qzalkmjw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zaikopbz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3weswwako.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3estcvuyh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hqjogebe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pizamauo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tpynowjq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3oltdffxo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypbcvxdm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jziwrutm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3plynckam.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iadeoqnz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hszjzmle.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sqcivwju.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3apcgmeyk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3txqyjqvp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hjfkgntw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fixxjmyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vshfcajo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zwmjbowg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ehnfcawz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pjdsxjbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zihxevos.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3toikyizy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cleqmvkr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dktxvfkg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3idpctmci.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gblogjop.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xycrmmvl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pjcpmbqs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3joblbnfs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zgyhrwfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpxnrywm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jvdjfmko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukglcsby.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3fxzanqdd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qapmdtlt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ynquyxau.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wnsokzmw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhehcud.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3utuhzcea.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pwtiyoyi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfzugiyw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvtjokkz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dxnnpdwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cetzmnol.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gyermzws.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ktdnngxr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bpumsnps.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpgebhh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3oznoytwq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lvsnkspn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqxhfflf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wbvhzcwz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pvxamrxn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tljzedwf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qrlnprly.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bngunqdh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oiylnwhr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nxwlehot.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wmszxwgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3euscwugp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hruthves.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wbttwuqf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uqaesruh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iqsbbmvh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ejgvunkc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xghvjghz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kfkfspgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mhaxdwbq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3auhuarcm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dwizhavk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jmvfjean.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ojwlnsso.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmvakjvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bozvloqj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdznmjml.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3coedlqrm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tiiqzfyr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puithwvu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kfaizvls.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ropzddal.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tnacpwmu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glrvqgzf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efypkohl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ubtyaeqg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdebbmkh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wocolkvy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qtcgcwxo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cghuaouy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vokfqjgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrusdkdz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3krpwhvfb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lqdtmkej.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwoykdbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jvkqmuwk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fflpkgic.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hxvvplnv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pyhsutpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3txfkniyi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tawhpnty.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vydlvaox.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qmxrfzek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxvdkmo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wagovomq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3sikttttd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdmwezz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vdsekgig.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmxqpgdq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aadfhltm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nsfyriwg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rsreydcf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3imskgjgh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3seuqoica.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jidzgolq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qvbxgxzo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wwujqxby.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeewgzto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljiaapxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyhibmq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwenpeov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3blkrmsce.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3muyajwng.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qopslrms.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfcwshei.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3grqonuff.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynywmtcs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3esjejcky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwtrgtom.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwxtnncs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nujswtsd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3txmwqnvy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znlpuolz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ivskbtlx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3svtlixlf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3eoddqdxp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tkrmugmc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xlnpfglz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vbskzupk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dtwtjewd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qqsjjtzi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dfgkfosd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ojwhsxot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofqisbve.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rrqgyhvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zknjrjdi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vrrxrtqh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dwfzukdm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxcgibul.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3trunavzx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gecqchaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzilkxpv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lthveabs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ckeocnqv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtficcaj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jhvxwbhs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3megunexw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ihihtxwp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jrfgheuw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zsoxjmid.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpormgps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lzyvzdpv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dsksilel.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lppiczeg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ocoxacdd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tmrlsizz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3twrokqhk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zlqhxopz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgjfsi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ftygtyes.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uevwnksz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hrudvdmf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pjbpkszx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mpdmdbel.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ovjfihdx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbvnfcfd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sfwagdir.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqtvczy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qadxuuee.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3omaynmdr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwclhlhe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lrktfhhu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nmwxyxbm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mkojqqfl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kbkjvbcn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkvmwqyg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tnkptctn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mfoqtcsy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3duigzkhu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zimbilas.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mumjnmqh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3eassqmhu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3inlvxxxq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3famvkghj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3axgrodjq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wbgssydz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ulxfiqnx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3eugaurcz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3swrpvjse.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hlgwlktb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qwzfgxgv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fqejjvdm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3thddmjba.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eronhase.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ewpufszi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3deugzqaq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wlcvvjst.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uzqwqfwi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3robxqktk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rysvvqpr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mrbyjgwe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qymqxxvf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3umberhng.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3imbujelf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3svxkqstb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3efbhiwix.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ytqnndjs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bpkqtroa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cbhzncos.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lhinwiro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujydutxo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wzftuagm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3olfjpdkg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kmqwljjc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3waqlbtaj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dnhgctsm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvdiygi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3losdhiol.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3iisqbiue.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xdbsekoj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sswnugaz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fqxxldxb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3easrnwum.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mgcyflbo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ljqldimq.html


<!-- 参考信息 -->