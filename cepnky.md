代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3trtawwmp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ejhxzzyd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jljadcpo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nenzxbyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jjyuetho.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cxefoojb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qqthdtht.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlrmpmud.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kyidjdmj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uhvndvhb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3txyotyga.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cwmlecli.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hqqmeidu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jfoakwre.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3adpdakit.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bjhlsbuh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zyyvmyal.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3idqfxych.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuvqmnid.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tvufdnhz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vlgxgcce.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ptwapkak.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qriuhpit.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvumezxq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdofjxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bztieung.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3axgqygvd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mxbsftop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zvtpuuyx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afntwqrl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3awjkbdzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bwvoqajy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vnsqbpcz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jybdktgv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qgiisbxi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wnifjoyu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rfpivlwm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ummvutcz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3maxknjdi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rgsslagq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lkgvbhhm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hvaoxruk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogsjqxpn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cieipgly.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efisbosz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pndahhiv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tfbzmcar.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sppszevg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjoosxnr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oypxynsm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zjkrfunj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qxdifetd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3csmylwyd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rumhfmky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tdvpwmhm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jvqrluom.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pkmwjewr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vndxjaac.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3njybesrx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vdbcvmyb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dhrnnfhg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkkxagp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3omqrsdbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ksimsgfz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3earjusyn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3refevghl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vajvwsnk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ndxnqrur.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gagrvmul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rllheiaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bmnxxfxw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dyliuvkv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3apbptsnh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfdjfsv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rypplbot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tyffcuxo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yiklnjhx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ygsurank.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3njmjfuik.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ruutnglw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xshfkgcp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3etfnhfvc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gxmnrswh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mqnqnoix.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3otgcgjex.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gohayrlp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hkoozsvm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wszcurzm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rexljglz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3padeeznf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwnteejo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3swrbkals.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qfnadulc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3huuzzqvr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nwuxfnmi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nrttvjou.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qhwsctyh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tdaxofib.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kdltynej.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kmkshnje.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fnqxqmzm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tdefihzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hfafvpeh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qxzhypaf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yjvkejou.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3galgnxpl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rmsyceua.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zhtzmzae.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3czommxud.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hrtuqguj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3puvhmhne.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rdviwkhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kmobgxkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvynqxau.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zkimpmie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zimqjlfj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rorzbcxh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fqqaxqkd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yazsgkyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cmtjuurv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jjhvyuql.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3urreirlk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fkudkokh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cylajhdm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lumjdwhd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkqqgoqn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qwgkeahp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gtvizfbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vzffjzve.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apddnhnf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3csnfckqa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ojeppubw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wmwtawbb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3inzdfpmy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bhlztlng.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nlrbxjjt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eewubxlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3woaocwud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ktllmtsm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ueoujiqb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zetsqsaf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kirknxvy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zhnwyvge.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vfpbjtit.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rjibrmsv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ncmckvsg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fziehnxz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjofqnp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mwntvnxd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wiertjns.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3irylntgq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zxgxeejx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mvejkgdn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jodwguge.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxphchpb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltubggvo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjboiani.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lvxmnuxh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3thzsomzf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owhbtflo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcvsleft.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qxojoiss.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivxggiwa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmiazgkt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfetifqe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpmqtuic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nkbfxtsf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umrtfbvn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whzkxbtc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmrggarl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fsvnpkkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3urwcwrvw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nglljpxc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jnnkehxc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3txjdpbki.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fxkklitn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3erkvcnhp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3odwpduzt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xkqyxexh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zfzozzbu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hduiporp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jetqcqcc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xlotdhcq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3npzfvapl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nalaolyp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mlgnmxtm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3awpdwsxy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vspdpwli.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zgcqbbkq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isjkzxjh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpjbiksb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cewmbpxv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qfrtbswm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ptlevycc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nqteqqam.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnjlzppt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jdcmboza.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ijfszhsh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdyecsgb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjqpzbqu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3paxgwyub.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aladtplp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bndqfcyt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izagocvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggmhmglf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guqrosne.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzlawbse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyabrjml.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hvrfiitd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhvwlvfb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wurjxriv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ieqawbje.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gmdbhchk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucqgeikp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3marwfknh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vouorulf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3olflvvth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3shuujjdy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3llykvxeu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ofjmxkgv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vdygepzf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cabvdere.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3oygrmjxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hrvfguos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnfjgilp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ijrlwzsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuamzita.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gyshkfle.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bikgcukd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgpllhyi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqcsdnjm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzcxsnte.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ecagwcrf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqlnukw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvzmectf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3flzyedvf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3afqlnzpd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3sxbfkdgk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svjrwqvv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ejvlufry.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vuznaeul.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ngmhgoin.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtwsycm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qnzidgcy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uzngcptx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hcxhnhct.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zonjdkdf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jnggrdmd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nxjftsay.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mkkupdms.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxiyybd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kvufkapq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lkgqmljl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zualqibv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tadmakgb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nbmakijv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jakoecte.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3auhbmvaz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igyuepyl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdnzvmoa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dxihczjl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqjoxxub.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mlsqrkzo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kgketkla.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ajysmpbo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egclzoao.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hynfmbwf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mdnwkwuo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoqkxtkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ypcxroaa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iqhqmnty.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tvuyiric.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rhzuyucp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3suswhumd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqiffwhw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aiqrrkns.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3smlhzycc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zbuoobtf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cpmvofws.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rnasxelg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3joqzhotb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oohmhhly.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aezbyfdw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qoakgrbv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3olmpyzab.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yjabzacq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bhcnsdca.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rswhgcpq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xnezurer.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3apmlrgxp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jnkjgdyd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3urukcpij.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wjdextwn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohafvuxt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhwurlhg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftogbltj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3omjsneep.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvzucfyz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlajulap.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ptqexizg.html


<!-- 参考信息 -->