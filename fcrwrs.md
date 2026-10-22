代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsntxj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wswjjrpi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cjfzhlrp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2grnntfes.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ogqblnpm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2urqvtnhj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uadomxks.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2etqxpbho.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rjxpmtgt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cokdtaay.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2riujwlpd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2irsajemt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xfsjpidl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eavjeatt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pecwkzjb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2onqkpalw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zamfsrep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whlvtqji.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vkjpfzgq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mkhujcvu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lyicdekx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xlhkquoc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxqnbdig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pjlrkkgf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xazdrvik.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ppndsbiz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2srfrrupu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yxkcifgo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tdcaoluj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wbeaksts.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jdzewcgp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wexymkjm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tgaelyiw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tnyrzqaj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hbcegrzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmwljak.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2byxnpcdz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhsezvf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fbqejmpk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sslfbcne.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pihlslmv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jzedhhrj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tvxgwjgt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hrprhnwx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjlhzeza.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lngdgtwm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oktorlkl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ixrhzjpq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vbjjumxw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndnynmwd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xlycociv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqbbast.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhuaanij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yotbrgxn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2umryssoo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2sooatzhv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2crgmzarf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cksfbtgq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2itnhhtgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lphtzgvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpovho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ohbghqdg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2txhpqgol.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zuaycxed.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2myojmvhi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xstttbkn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rxctpqxd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vyypipxx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iyncxotn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uvoasvws.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fyhnedyb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhvrryi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lwmtgpzv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zodmqdme.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ajijqhtk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qiodixlq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2samzfwns.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrlhbwgg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cccifieb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sypdtuwx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2oydqvxrt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2weaduopx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2titcutaz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ouuovzom.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2loquurgd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2btwdxmza.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2feuwrfri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bbemcusj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhuqvr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2geianqcp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oksrufgj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2agpqbqzj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmzgybxr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fklwywrm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ndvpkrms.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rosxxwel.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yaceiwaj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yincmlvg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2etarzcsc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qrwepjmg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2icanobeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmkxqyxw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wdhjpdju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxsymxth.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbucoh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sglgrxmp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oxncovyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vitjswzo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2laarroxn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2otamnkzo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qavxvxze.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evaiioel.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2obyapkcp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2duxcolkg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xyzdgatr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2aapptrvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tfhlrwfu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zrtxista.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2baxxrwjy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2auwjitks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvnttyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2limbgotp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2apugcsux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xolwmevl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zmibmuiy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfcgruz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ftbbixmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ayjfeulv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrzgutj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2befzrqon.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2juxddkzi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2immezzkr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dtytmfth.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wupxlabt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fipckswd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yofexywg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2htbejxbm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vorawini.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ippcuejp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pztuthel.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nccdpyej.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zzmtsaia.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xsrluhlq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrdjecnj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycrilmfx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2beglgwrj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kgrlzyxx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igrbudpq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aketkbfh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fgrbkxnm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwixxdkp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wrtwgwuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sofbabre.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwknffzk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kagqukhs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esdoqjtk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owcjgpmb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dppgeirw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kjildvjt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kgxlgnal.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2unbmlnmv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uvalqvwl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nynkhgti.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ujuhwpim.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcuhmch.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2aamjkkrf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kxsmeedx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xchuqkyt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2losdsuwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zihuvwqq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cuxfkzfk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zbnuyope.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xndzrcgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlvzpxri.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eadrvutj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hiqtjcfy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bojqowtk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czfoigwc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zsjhbbhg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kprnjvpb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uanpbhje.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xnthdbjf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dzczmplg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gcrbmnmw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2otgjtlun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qorfnxey.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbdltjbg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qhysvmit.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frotqrue.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2byglfglb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2slwbsesj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kaqvlpff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylbdyurm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajkmswfc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zyaypygu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aiudrtlj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shiksqlu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssaropwx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwsdgyqw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwryync.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ljeyjjqi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfgzfwqf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zhpkcbyy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ecvnswez.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2nsporbuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nwciwexy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zbsjheew.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zkjnjsdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sorxqfip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vfldymuu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xdcentqp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hpypnfdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfamzfpx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qzyrmlbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfynkhqx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ihutvzkv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2aajabbpz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ztbodjix.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfwnvmqi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zfiddhwf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glleyqww.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ebxdsaip.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eefoyjte.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nsdailea.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xatlrjei.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xnqnlxpq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svvfkkfn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtvbnln.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2datjthwk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dnuwbqmi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bvuqcnhk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgmchstv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmlcngf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wamucqug.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ajjtapku.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ykdxkupu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yfaudaou.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gkuqtpmw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2crdlzhcz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2evmbemau.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdrjhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xdlnczrg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gjutetfg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kvxtbwgy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2goeyxckc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shyyeayn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khdbrobl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fqavwcgh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hmojpypj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2haoxrhte.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ienmvnmk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oapfxqbl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2acrxawhd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvpjdemf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npjdmxej.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2izpewqtg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2alielohw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xdormoij.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2furhldux.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abunrzav.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zzwatywj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ciuyfbjk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gshjakdy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2djhdnqci.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dpbdtgur.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqbovab.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bevrteea.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2svmabogm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vxonpgto.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jcegpzjn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jdgliykh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vmpmxjvq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2beqdfdau.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jmskpwef.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lyoghkxz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jmwahpqc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ogwrawbb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vyfdrdep.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ocbdexze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lougiyro.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lbrubgnd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uhrjbnas.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hspejjpa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzsyxoet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ozndqedl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylrfdldg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2urebpsnd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2arpidteu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ndbtaxyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvrrbhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kojfdvsr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2byjzsewj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fucdptiz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wzdxynwi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jlobiaiv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fniohrel.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lfrysfch.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mymjzwrn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bhhonudt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ubpsqqoe.html


<!-- 参考信息 -->