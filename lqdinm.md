代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wzqogdxt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ifrmljod.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dzkkjrwm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nijneefq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mgxjezcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zwjahare.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ltpndenb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xfysrabd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2brshtenc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxbymwi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbuaswcc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2udafbjdx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hefsldgb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wnmhykat.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wadzcefd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlgztqsk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzlwheo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ctissmfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2komthvcg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fsgucirl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ndipqbfl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2spwrnapi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2luxompoc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rididyir.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2geeuratq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nuffxylh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cskkddwf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mifwzkkx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ohxnwkms.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jgngbjge.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wvchhskr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ibwcenyk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2aerpxdyd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqooakj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nbppknjz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kntkmxec.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rmghvxic.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yiupxiqr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2czyreuum.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfiwpvdr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xqvbhrld.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dwepyucd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tjqspmlb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sqeewbmt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plqcuzhp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qjgqxouo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lrmpvzoi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dehildez.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yiumomvl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pgiesbed.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sovvdsyd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mawvpmzo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yivdslfd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ohjuqsvr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wkvqlktv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nytxhtqf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvamcusq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qjbyhdmd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ejeyntvq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ncyozcyy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jgcnsbcs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dookdrrx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cikslaut.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qhozegqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cwepkgvu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2latkvmsh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2aadvhyyq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nejwmweu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ikckmkdk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uwwmsnyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smmpbzfj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zlaqfqhg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ozirxoge.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fgwmdtal.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ipfybxez.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jeqqgkit.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qrjcqwmw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qwcpidkf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nrgindfg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgqsiiu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2istuvnbx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxogcsx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wrrbnpsm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iyantqfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2glhmquqz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2otdtiebc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2igzhhtoh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgwklbeg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rlvywxuc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tofvianb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gpsnzvao.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lwhqxofp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cmknywll.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kdacglph.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lkrypfce.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dhmtlmkh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2khqyoxts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mtakaxwt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rjlrrdwt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2krmtysgv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2czppkowq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nkjtrmur.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnthva.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bskffnmd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2drnukqfc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rxciarow.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uzdjkivi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2manwkjvx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xxfiakoz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ykdzdjrx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktkalhxg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eqbpfbez.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zrclemmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrxndltq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxvrhvsy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgvleibe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oihktegp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jgajfstq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tpopxusm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbsmwyjh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xkubutym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghutkkpk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wuiilqjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkytaukj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wfhkeijo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfzcque.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnocdqjd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zvyfqmlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lryntgzx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivqngcci.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kbskqhzs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrxtocpy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivftifpo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yumauouf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xqlxyxph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvjbalwr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chydhxoo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kmscpfjs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvpoopp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jvialfsz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rrbgktdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2umqimxve.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2oemvilwh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aozdlrzz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jkmshuix.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gfwndqof.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2phofiwud.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lzmyhney.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2emzqazne.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nbgfaiip.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2twyolhhd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2paolcbap.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nkqztkwx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2roytpfns.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mvpojpdt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sujctkya.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zjfrnhgf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2usdepqkq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fnhjlpxx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kxgviniu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bdbpdmbt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kadbateh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwavjfoo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkwlxxiz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqjllvvg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uapsxtcm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bxwzxcjg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytsnxkhx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khodnplz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gckmkkes.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpbbblzm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqpibgjx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozemrvdj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qaglvkok.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yauyyhlq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zixqtgan.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jawehrqi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ipsjaafp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mrtcrlqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xcuupyuq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wnvwweft.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qftbjymc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jpwoswuq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vshbmwng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dmamzkhm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2oemzrijr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lcyiaigm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kohhdktc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tnnthmxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvjhgyph.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2alfmasaq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ttixocis.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2htjrtetw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kxpxsjdz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ebalizfm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2prcntskx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wleqmged.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuixnpcj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmqjwsjb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fjwnodam.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pjyujwzu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xrxdobxr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xtcmohmm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frcmaczh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mwmteibg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qxjinwnx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtvchxsc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rmojlgaa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfsjzxfn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvokcsyp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nvvdilwj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owdmghms.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndzheroy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ueyukjsv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qlijhygy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcksxufv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2phmdcgid.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rowhrbsq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvqoebcm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffyptbsu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gojaigrw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okddafff.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gwknybyp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ggomuzhj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2emzfkmwz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jdohbknc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wluoxewl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ysnldmlg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zkihlvkg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rvfyhinh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hajijpod.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pcxkbjhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xylzzufg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mknmlzua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vycqjrpb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bjzpguow.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2syrrtyev.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbwrqwdl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuugojgc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uzcoqmwd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxcywgwt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nzzdxawa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2adxagizg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbwcvihn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgbgyuny.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2djzjnnoj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2odnpwdou.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwvjojo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2phdxdrcb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2flbkjzbw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qgjzyyot.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jzgsyawx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkxbxr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2srsoharv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tvmrhlis.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qenhfusq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2awzmszvq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mrmfybxl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbkvunwi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2knfteakt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rvgukqed.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hiyictxn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nmlnkmfd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2opbyipqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thkutims.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpudmtfp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2batefkmd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qamjujjt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eycfdprf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fivxnokw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tbdxbfld.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dkextrvh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2usrvckmx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lqkhbkak.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceujofbs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qqcgdmum.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvqesawk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qcycjdgw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2btqxuadm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyvrzfvg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lecwubjz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nrvxmbnj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mbywzqys.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhrdtcfh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqeikzzo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zzpllxcq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2eflvhurx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwiezueq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ltbptdtz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qzyuctfe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2papgytyv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fxmknpai.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xjbmpasl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lajcaxhh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vjmrvjkv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2evqpsgxa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lenzcvda.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wxbtvjau.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2drdgexda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zqjtxqnu.html


<!-- 参考信息 -->