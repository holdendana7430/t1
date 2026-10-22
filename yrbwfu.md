代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xfmnshgd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mwdrdvxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sugtcitg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxtcjoid.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ulfyrwpu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ujqlotke.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2edyuiwzj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqomltx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zkqfdzxz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dmdwxcdb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hzgcgfis.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iovmsyna.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qiuxrexi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2djhuxfvf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pztwexnv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2imytaksr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ohxohuza.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vfysxsog.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gxialviz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hqxbyyef.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yfktlufx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxositgg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fukfqqls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ltmxaulh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dhgnhayt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vvnmqeqg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2abrasjvm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2stvixurw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oklmcbgg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xyaxuinh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lhwnwbcf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjviclro.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bodejnfe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xxlnmkjk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmxwblr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hceaqnzo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vddtdfbp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2srzqfcmx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xmoxkdqu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzpisdi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwgtljq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vouotfgx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2serzcegj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nsoqquci.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2swbnhlzq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ynrwjbhx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2opfpbkzd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fajwbkso.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvysboyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2otivxcfp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2aechvxba.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ozzgdves.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvpruuq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gsdndouo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gmzqovpa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gqojuuis.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2imcqaqma.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uzhsqpsf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dfmqoahv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ynqtkdeg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2trjqkfcf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxvoxrac.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2biszjrpg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ejdzobgz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hhhfptmi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmmlbmte.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dddauccy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nykycvhz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2txzjpedy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sscustma.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sddglhnh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rlnhpjdd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vqpdtmgn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rqmhqqzp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tzchqhnh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqwfavdn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sllrnuvl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2grhliqjd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ivinxxdt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2itnbnezt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mdfpiqkq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2shpwxyir.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2eyqxrnea.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2prfuiynt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2svuamuqc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tkhxufot.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxbnlnho.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lbziunbq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gnjaugyg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lqedrtud.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mkatptmc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gtmkjwer.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dijeeyfh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2icbhhbtv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2msdwfbat.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lansqocc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ufddrypz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mlmyguct.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqynzenc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lwgkaffx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2knidnasr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2saqfwuwm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jicnaylv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfgauzqx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gahjwyad.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2oazrfvca.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wbmmqdth.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pysmpijm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2snchcspl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evdbkftd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2frlfrsqa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bgrqcjol.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqvzlxwv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hinvxgfe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zvhokzfo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ofrubegm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2migyaghg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpsftedl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rnbjlamg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqmqlskb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mahmwuew.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dojpkbnd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kjpsnezz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jnfmmjzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2omsbafpn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2njbmfllv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pvskgurl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvxbhmzv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qqsmkcjt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjbmgpwq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2frxgvaed.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vyowbyui.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lhcxvelr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlryefsq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ogefifms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rmvptbnx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2biogalqq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cscebexw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wnbaksnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gijdjwvd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mcbnmivu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2glthufnv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2epfkfwwy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dnanyxgw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpyptfh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jtaksltp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lpxihcyh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2txowsapa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2whhlkbge.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nsrkxzud.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gctmwdrr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mvrybisw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvtzrzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bqaitkqb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kksobcic.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2laqzburg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ctnxllnk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kkqemzyu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzkrdyol.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eniquunl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpwtfpaq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fsootdyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2iqyacpws.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcoaycbj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixqplnmk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qffdaicy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxislpn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yemxzckw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywrhpqka.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcmrckho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqondvrm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eyxkgovg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsrfudp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krijjnjg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nzyxvpea.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gukcfgip.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iisdokki.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oiagbjxy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hgudvmtp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mpbhqxog.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mqcimoei.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jjszchcj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bfivcdaq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oeuetzfn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufsaarnr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2guvxwjnz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uniuqczm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uxvgsnej.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2owlybfkw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zmbbsimh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ssxzxzao.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfwvdzar.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2znaaysek.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxwslj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvwrbueg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sdhvcfag.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2llhbsbdw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yakmmpne.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nfakhosa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezmgoykz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kukcpwsd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cigjgzis.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbhvgcn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfuofehl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udcxvejg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwveivnj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2echhoijh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eunsxckw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqummwee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aynadgqx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qejwzwxp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2drozxyjf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhzsjiua.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbkzwxms.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iymncbqv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rxluymbp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pgsvdtom.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2crfdqpgg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bhwhbkdz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2iywbpkmc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2saksfilp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zjyrhogs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xybtmxvu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fexfvtrm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ykuulacq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bpdduboq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pvjxjydt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hspdmedu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czfhmlnm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2djplsqzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twiuzavr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dnmzvbid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qqenwtlk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwsrtads.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzhbsyby.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bufocgqw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2npqelrcy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ntxlgxtd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ipekympp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iukjsiig.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txeqnsll.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gzbbkrvz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djngsnzz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtitbz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxroddod.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mhszkaze.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ezekdwab.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cdfkszbz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jykppoli.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2frkirmnh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tehxjtnk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2exgdiemt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jmewfkzx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iboiylyj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kritespf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ohxozonl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2crttylqo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffpotvre.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tzpaqlaz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2atvjqlck.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2guhurmug.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uggarrbz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aeojpnph.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mztzgbqh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gwgitkyo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wifxsofq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bsmuzpio.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bkqfhoow.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mnhszizr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rsqnzdum.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jelvgaxi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2haqterak.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jucaklws.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lhgnkuab.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncbcssrt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2iedocvwp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jifvkvxi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qdssudpf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ssdtbbkx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqxjkrjp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mcjtkgdi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuvehmte.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mvvpgpww.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjczgw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2exvsytaf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ekdutfzf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wpbtrwda.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2isfduofw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhptdsaf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2woljykqn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dzarsllg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lisknfaa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2aoohyizg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bwjsqgsn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lhokqyus.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vjtoyeub.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojfzutzz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcsjkwdy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pweydzjl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ozwybvyk.html


<!-- 参考信息 -->