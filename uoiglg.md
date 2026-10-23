代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xhhnfves.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hzauibgh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3irfjwpzt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iqoouppw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nzvcsarc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qolyhewe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3axpkrikl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ydylczau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jvikaefa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rwngksum.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dsldkwyh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eixiykiz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bvslbjuh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rqspoazm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gxyjzlya.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tfqpdlcu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cyudymny.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dnadxpcj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pwytssvx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbrzrlu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wruefqbj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cffnumjb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgxjbiob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gzdnombs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3syjfshbg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qjdclcnd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wcwzssud.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udkrutug.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3eysqijek.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3omsvfvtn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlztytsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3retupfwk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqamnduy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aaatduwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qqazwjza.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfoypfa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tcsetlwd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vcdhyofa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwewgmwh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vjlkeewl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkekmw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3szylwppk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ngdeyyvd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hsvzawve.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xrxihaht.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mcjeivqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhtgtrw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3brpqhcqv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pttcqnbe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hyrlhakj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xfxfgbtg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ojtmcrmc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzaiwyj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rwkuurhz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jobonfyr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhvuno.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tmmcftlw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tsdinfwq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tdxgeess.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fjwftqnr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dzxuevix.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oytlxzwi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ihzxhcko.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3omesdplh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xnhddahz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kugmcaca.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3evkgbbnq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cvqozflz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dxzeqjuc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ffptlljs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oxntfzwd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3epypsrdz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kzsshslk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ckhiydsh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hhinbdqn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnitssn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yjdfohpo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odnykley.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkeqwjk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yklduymi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zohwkcgw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ikryfiag.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fjkxhasb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzyautyu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kzdsqtii.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3clnqzyru.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pgndarbf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ccahpaic.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yyrwcvbv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xhdkzfer.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xevezuqr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cnsiacsw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mkuhnawg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hswpfzju.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sinmvebr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycasrcvn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwycudto.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qvzvplzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rnzdxscy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gxdkllkj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ealtbseb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lpamuasg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yblrdgqo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pdfnyadv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gpfukuyr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vxbnlyeh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hwospcbx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iatizwmy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3odqhfarw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynuuqmzd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yljazzzg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vqwvlbxr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeihbgid.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3maqpraah.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rvufjbzr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wtflenby.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oqzcaomv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atpdzskc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3amnmntzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqtdsvpo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrxeaaoa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ubygwlij.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3airuywip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zuzsagci.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vdvjwgpn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qsvioqic.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jvitgbmj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgqutcer.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxlzmiww.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3eironrrl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3agourorw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nerdztjp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cgyzyrps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vkwafnjj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3adpudxpx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3peoiuukj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ddbxgviq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjyatkrh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3juoqstjg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ltdypynm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lepfhwqn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3txvdufpc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jmwbbvkv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bdmbjahn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mbyirtpu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pgmophdv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cxtgbpjx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yaamuhgr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dnfgzedc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qszillog.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ukvxkbgr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlwoezlj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fzilhmdr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gxnlanpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjgxvbtq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ffwrbgye.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nnqwbsta.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kxnnqjuq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrkiuowx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkgnttyr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krzssegr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mugfeppt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bmrccyip.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tigujmqe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjaxxgin.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gbefepvv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkbayupu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fkfvkyoe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfxarpjq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flmgrnud.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukmkmkdv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjjjttbf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lemdetrl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbluhian.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nytgfytd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mdnfeocv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dacodfbi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3prncpzfv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wmvatpiv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gnspsevg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jgawprgn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nhpwfrgk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsnnsx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tqacaqwe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrxshvs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kvqjnmsm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vcctwhsl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yujvlmlr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uspylezj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fwyrfmdm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3unkhlboi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3znowawqp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fskdotkv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjlyxhgn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tkslqapi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dbvvoqaz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oxvraxkm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kbahsqck.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3asrlevjh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wptjsjvg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jlqltanx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hpjzhwfn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjifhapu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgdccoob.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noclfgxk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbfpdcy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tqrctwdy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsqfeton.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3miiygtvr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fogocplx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ehdbsaen.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nibohgsd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cwyerjqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wigzfexl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xixyuwpb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gvwketex.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wrpyocxg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncftjymz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3urmvyzvw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3okdydgur.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xabcjnnr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ulktqlex.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3phoeftgz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vgdmmkbo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3uytcdnzd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3clnrhxey.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zdddigpl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3goszbgij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfszsjgz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vpbovfds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzrbscvq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pshgjvgc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ruaerliq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3czatqoba.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ezqyqwbb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3chllfrhe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swubisfo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3pvqctkpe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vviqvnuf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ozrdwitx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmwnsbay.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ohoizedx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ktawkuts.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qcppetbq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awpftagz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3doevrqzr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3niqokuqz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3codwzzog.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjychswo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jscmgily.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xylmbvdy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zsqbbcqt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ldtjyrhp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rnsejqld.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nahjtaup.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xzncuwui.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rysxgncr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dukexnfe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gjseucsj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qbqrdlgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zuivymap.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uoladgqv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3krakwmlr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zphhazpp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxigxli.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kspbihum.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tftolcpy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3onhkphyj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3doetpjuf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyculytl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3elzmojrm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcojymwr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igcxbzea.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rypvdcew.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3oefkxkgq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yfxeeold.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jyjxltrs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kffoezvw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zglsxicl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uktwzech.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjayflxc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3semrglbe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3eiufojyk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bdlpfswa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3syjouczn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gaefysym.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rkglvlkk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vgxioghx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hqvnaddz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zkqqpjrb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gtqjwyna.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kggohhcz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rqmeffce.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kxyrivfd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jhcnvgow.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vyjwxzlf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yatjkkxx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3umldkmkt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yuygkwgh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hokpnqnk.html


<!-- 参考信息 -->