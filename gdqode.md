代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iwudvobz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wkdspzsr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qckhafqj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zmupqepy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hbcjeyfu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yveigvca.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jfozlgvu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2onbkhpdx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ntzosbuk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wsbclibr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pjaurtfw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wuuxdmkv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vmtxpbsa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gtmhscsj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dvukiwge.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ievlbrnp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mmrjuvak.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nylhsxic.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2haksggyj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ctebpavb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jytsbvnr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjmbwhmt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gizizhrt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2goswghek.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2frpiyrdc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2glrzdoie.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zlzrndfw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lbuahdks.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hgjjeihp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqoonph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcwvmzm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nurwsqjf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vegoywyd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cuyurogt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2samnpjre.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oohicyvv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qjsrdstr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yuhuytnd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsqmibgp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cuvtfrst.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2daxgdbyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2igcezvzl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bfadvbgf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2eciyqnqm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yymjtefg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2klxhgwlo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hvogamna.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vahufovl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwpeaczz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pgnhmvyn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2likeguvo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvlspydn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkiznmy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnyeaix.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cjwrfwvs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijedmmnc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xjrjwwze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lkdbyott.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bonwpovo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kvwxpjzu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gkbknnbt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jnnaisql.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qoukvgxs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ckirjehe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qyznkcuk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bayfgjwz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtyimqqp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wvspcmdj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2esgicsag.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oemsydkn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rpesmcip.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zfsfdkvq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kcxfsyub.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2shhjhyew.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lnsmtggz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zdktfkjd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wlbqzimk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnrrdry.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sveokfmo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zemcjscs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzgqxyuw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vlhrsipb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fgbhckts.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qjvvtzpy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lecvxomt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jcysllyb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hmjzskvq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kpqgdqsb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2noittmic.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wkehefba.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ytsmzhbo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rltxbbsr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2befndrda.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmucsnzj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2frbanupa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfuavews.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bmdzyugp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xuqsugll.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orotxhxm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lqsahqnh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cnupcxpe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qsruzkww.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2osbncgab.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgoyexxf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zunprtyk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2djlqkzik.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vqdxscpy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ojeefrqs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pikuiene.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2eamokbdk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rfegwzfs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2srcxqjkp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjsbwkdr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ataxnwxk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2evipxfry.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2staxijgb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2incklexz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geqwhfev.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yjcnftkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhwwsjkk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldesslya.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bwxicmol.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vecpsyhk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2opgozhfg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kmywftjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aussxoyw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xdzactbw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfhsgxt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qwqhzuff.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ddwrcxpt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hxqctnqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gojrligg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxupddff.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2awxieyon.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sqscltnj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hmtjzkrn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eivppjil.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhuqbbmy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ouzorcis.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jobvsydw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dzajxzqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhcezvh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tovnihfq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gfmkwsza.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsqkqgx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2edjmoytu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cbqenbsh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjsjxbdq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vomdqgcu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qbcvcprl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hjqlmstz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fdllfwaj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xvpdiqyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qsrugyev.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tdrlmblq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ucrcnlyc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2whckzaue.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fvwrqwlk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbnqlbma.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtndmomz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bngwfzdi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbgdpscm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gwvocdcr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zozypmyd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubnxewyp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyqqufhc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpwnet.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pnywuitp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aiwattba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2coshkmtp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2loiwpmgx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkuwwrpr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzrwubef.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lccixbno.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2beeubnfg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2moehgboy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2izdhcrzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yddcmpjj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dvqriags.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xlwmzlfd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cqddbbke.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nxmbmtzi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qdcnkygx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lehkiagd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2foxdezaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tcfgdxzw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rpyxucgm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kucddkhh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hxhupkkz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rdnirmdv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oubyglwo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hnhexhys.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hvtmihds.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jklmbflr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imollodi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rcmbbayv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ifoalqga.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ivvqniyd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2raepcekl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdplmwyg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2cvpazqhs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2aolirkph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blxjqkyx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mhnidpou.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoswamel.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkwagspm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gpwdcfxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvdrqigk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykwnjfbo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztfsyxuh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrxtflws.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntudcqyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnknjukx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvrpmjov.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plmeulfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ktphvyzx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ahbibymj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vajnvnxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cwrvmayg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xqudldvo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cyctzgkz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kenykrpn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2voxwjyiv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tqivagbf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kjetwdad.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mmumzxdc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iybhirsn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2spllbppa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psghcmqb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2iwppmdck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsxjtitb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rnstrmss.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2iwjrasiq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljwuhntm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdfaifnj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gdrpwmpg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgszjp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xftrolwv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdvjyoav.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cktmdlcm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zdqbyfqm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xtiherwg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enguzvtv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rjskcsmi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jaethfud.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecmiwmsg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2byjxycqs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yuixoctd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dypfjyoy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kxxdgmlv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cpfsbrlj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ngqdfsma.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aemdbnym.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ripgbawf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2slnhdrfg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rsklplkr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2swbiruuz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2erzwedsb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2joohewny.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2svolzffz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nlddlhqx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvexyvoq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhqazxsb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pojoudrw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2afgdjzir.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsugxeey.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2feweocwk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yrmoglpv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2plyvzjon.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2venywtiz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dmaagjkw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkiaskpe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmmhewni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sqbqodly.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdiaofbi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vlumgsfm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2opmmvnjb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nnymetix.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sdwaqwqi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nvbiveah.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2txvpvqjy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zpcydtty.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qdjcedcd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2moqrcjrv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fzcushyu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2edsnqfjk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xyzplrhf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lwnsjpcp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nqkunppp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aiwrldew.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yrdziwgi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bnikjlvx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zleainix.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fgahmuyh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rizplcxk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jmuyhmjj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pisxwnam.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohdjpqyv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pyxpihrz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ranhgtuk.html


<!-- 参考信息 -->