代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpxhckic.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mmruszvu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2porokqaz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zztogzlg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ttcjxaun.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2htoekccu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lzpipjsc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cvddyhyr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upevyewc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ixhoioya.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2iukkegts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2geexalsw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ljpxioyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qrhtqloj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rtwbqcew.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aotcgrye.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qajswpyf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xocnryqa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zyobserk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2aahkddny.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ddkdjdpy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qejdfrpv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dsbmiqvn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dhjylpdg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzmskbc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rglrztpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xivkhzyp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xagvybve.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fertzsqv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fssjeuaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kqkzzyor.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yurjfini.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mmlvmrab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bnkkydgk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ggtdtupw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jxjbhlrg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtlztnkq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xlloynke.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qdywbnez.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrsxrfan.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oylhrxbz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kvakuzfv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zhugzkuv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vaxbfrwi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xatofoze.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mlsvioco.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zeobbzqm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fycytmrk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rqcvetzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycpojehl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lqljslnb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oacawsoz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2chxlzqvs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2iytcxkqj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eggltkxc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqnlvjk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mfmujgfj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wpqweyia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vncimvth.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2atajyeza.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tmrvwlvf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dotracqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzjliivd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bcvqitoo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wfrjvjbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ythlggqu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2htzrpnkv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ipbinfef.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xvxvkcrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rpeondej.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cwrdocvs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcuslmla.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zknouayi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ipxdyrik.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ouezpjjs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lubmvxme.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kcvwgvbk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tbtvreub.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jttdnsxt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzetshps.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zhnbwaji.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eetukivo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iibgshzn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wephhesb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gjygmqxc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fdgyqlqb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ayjrwxsg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wkhlzqfk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zeciirqz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzcitpnl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zflxfetr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqdsktfe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2alrdumit.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zqbrzyhq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sbzfzkvm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2apfuseki.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gnfkfctn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2piawlcxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nwgnmjfi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocdhguld.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2avfftfne.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tfjeaudf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ruqjmdxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mlspieuq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mmcjbpss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifqmqdbe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gqdmjmuw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mlzkxqia.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dcwnittw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2afjoiwya.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xdzptunb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2romkleox.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2flbppazt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhalcnky.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2euzakuro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehxpenul.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2btcopbct.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ehawdsti.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apqloiwy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dstmytul.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2llykahlf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jvviksni.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2miuullrj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chughfuk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdpusqot.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iqdpgeen.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sgmhoqmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnapncws.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2enkzcxko.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hhsnjkeq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ciozurpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfkqntp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ozkkgrgh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2djdwyanc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2judnyjpj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rkchrhxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kynssinq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yecnldcc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ytxrsspy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2spykvjbi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bukoyith.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tgozulor.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tksmohjo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjcbduaf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yyyysgjd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rhkehjcc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cmbvksrv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2plzumria.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jzctanjx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qdrcnwek.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyscwfk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dfnvcckg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bxfpycgo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dmilzpej.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwfccsak.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cucoziti.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihtmlhzh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jwydbwth.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tlawpneq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kusxcjlr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcvkuczb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bpemhhpc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cflpmjvy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axqovcjl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukhqowmk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfwsgsmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nutwykjd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiwgspni.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbginaet.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhgpqgfy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xobojqvo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lgohebsg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qhdbzfiu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mgmppsks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrmgzzzi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xljpaisz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rftkmkve.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hdspnmoh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ugsrhxov.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2adywiltt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2oqinngli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xookgcyq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2liovomel.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bowidfid.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xyuplwxn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rcitdend.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vvgmpzlu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oijxqgmb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hakdteiw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgdzzynx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agztocln.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2olmgwssi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xxdyoepd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2enetxmcf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sweejqjc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoydorse.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dugkhhsz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nylqhjnk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgaljboe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqeejcnk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgwfktyf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjfwhpyk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ypfgpgxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxgqgfev.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvhszncw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovfyttgu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gmyniuar.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnaqzeow.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdgvbtcw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwcqeze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgbgjryd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iijzudwr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mnnkqfdy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kztqhvtm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2biulgyim.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dzexehlu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gktaudnv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bmfonclw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kviwwacl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rtjzwjam.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2svfbmqno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vklgqpcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2avlxuiog.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jhqudkod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tapwkzhe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2arsthsad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yumuliko.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rjtllipu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tflmfhbr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jviwwuie.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jxncvdik.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yufvkrwh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fktsacon.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cbvmjkkt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ectfjpxf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hzndzyei.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yyhxqpnl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ireraapc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suzeblan.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usulqfpd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tdtzorgp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilcwqarx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mtvnnsdx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dydcemcl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2luvlsqah.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iuojmazc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qdlooest.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xlxqifyq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gomewvrl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2azxaaidm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jwmclahj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2covyrazj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bmkastpw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kuwrdawf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2htetkisg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hqrhwvqu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrvwkld.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blqoycap.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgeyqpbk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwysmsjv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qmuhikqz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dvntkcio.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rxqdkxnq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tfylmzeg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bxokvrim.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqdyajnb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bsvnwrnz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubsjwezf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sqvfhtil.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mmbusexb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lajqcgyq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxazitcx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cyhyuonx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cwtjgwjt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ynhwcgoc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hosqsnwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2czybfagx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xldvfipl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bevwzmja.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ftxvsebs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hrezgdml.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fqenrusf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2llkzfmdo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ilitporj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rwxtkdnp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gqrzukcd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rapeibsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vyrclcfk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vchexbsc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2owznxkbl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hfvlgizo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qqrwioze.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jeoajqkn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2iywgfjbf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vglddxtc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvicvbdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dezjamzh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vqkvcwuv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bavjsyuv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ahynvgcd.html


<!-- 参考信息 -->