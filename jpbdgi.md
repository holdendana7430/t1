代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3prekgoah.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wdhvfixp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kirenmph.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cqquejhu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xtefcsqw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xjkiffip.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3infhjuja.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihaqhmyl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uhsbnztm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3egovkdqz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tducdoam.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fjngqdxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qsrwawcw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgcqkov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3oxoyvrbc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iwfyjjru.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3edprjgwb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3amvfqkpp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uinrjxfq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wvnlobah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ekplpnnj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3byhwexwa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jghprxnt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3isijroxp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dtllczdy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgmrdtph.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xletklnq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jmnqkneg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lkquqxnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ranvtfci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3haioefyt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3asnddirm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vcxxdezl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lieexsxi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eaysirdc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3evdayuxc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wfpyolwn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jkdkevvt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nhkohkex.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lfskhcot.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tuuvghvv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xwnnmior.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yriditif.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxpvivz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zowucsrl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sjajxnco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dtytimct.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gurqjzmj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ifoqbexj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vwdvyqah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bvzuwjyz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3raitipkl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrfhyrt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyxcvbx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xrzjinsx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rssfmzqi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ksaqgkno.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lhfzrzfe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ektocddl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3muanfjdb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3laubiqsb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xfupelmb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nlgpiccr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pkbodjlp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lijjaaxx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3axoreozp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xhfqcivk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3cyzydrfg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wwcgrkry.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cnnugdoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kxlefild.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpevaho.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rhxutsnk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nltwqmim.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjxvoslq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xgtqkrzk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ewfqosuu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yteoaiom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugaoyqka.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3syzztbdp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fjlmccru.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hddeslzu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3efmpylhe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3upcehnwi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jsspyilf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nxwwqopl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dmnvsvlw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbsnzij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bcfwawss.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulnntsxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3asnakmax.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uebzdbgm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lhzqcrza.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eyjfuajs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qtrvhqii.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3swpjcazb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3npygiomf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3drlhztjt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgwahscg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xmbwgjxy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iunmfqlm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3srrdvdrv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3focwgayl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vstpafuv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3icnquour.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvestvti.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpyrrpkk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xispnvvk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gsjnpzli.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3slmaeayb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgiqgwel.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jnhysecx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ntvjcdkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ffmxxkxz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wsgiiipr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3itdllmfu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3imkzwjoc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gbxvbxgo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jevkyitd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zswqpktz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cbwrhjdj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kngvmerw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oxvsuwyu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gaynejjd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3erhdjrke.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jkxkspkt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wyhgvuid.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ubcpzeee.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hpgwhytn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcmqntyf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dntvmdvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bncdwbwc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyobumqx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3eohxlabz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xghhjubm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ahmypufj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rwnisetr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jifuogvj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3otadfxon.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sptotudj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3giqseocc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3impvpesj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wxwywltl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mfqnqhqx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wvblqyiy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dlqmzmns.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eyradgwn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlkjodmc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ubbpfedj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zandbpcv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bogkxmhf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eqvxukxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kycbphjm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yaorhzdw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qprvnatq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3byfypzfb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbqfmuk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hddprsmj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bilvdxns.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3axepwdoc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hdirifnr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uomltmpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mfcxkawr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yklvhkga.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3snwacseg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hevacybq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3znjyhlsr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jtqqhzbp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mptcdgky.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtopyvs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfquxdyx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxztursh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbngjvnh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3byewzgeh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3knavyodo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxwhdrja.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlodkkpf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdavxbro.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndxcxizh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ixoyirdp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cumdbsiw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfentjgc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lxruyinh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edmfztfl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3micmytct.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yjdddncq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bqfzubex.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yhcisnkn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzahwseh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sovogvjt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ajmikdpa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ucfumzrl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qkotfjgj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kxdxsjgn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mdkpvduf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tejcusta.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqiwmfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zrfjgish.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwlzegu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qvemttcf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrtgzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3arfmqrhz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mswnrpsy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vhfjobso.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lzysnejt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkwosneo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncbyhcyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xedmmutc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3spnafugi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3reyrriko.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tzchujqj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcrhlqmw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ikbfnyic.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3alydfdwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epmocans.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnvvntqg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdubdzc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhcciemt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hwilanfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxpexjen.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmbtjurq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxydahmg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fwgisypl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmzresea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3akjxxgjq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwihdapu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tigwteyt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3izplpwru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jlaobseg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkmmnpcx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3piayjczc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dnshiour.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pchrhqfr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3siwfovna.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aqhoxpdd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vbpacvkn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vaffipqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xcyntkxw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jpsnwttp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wbwmmajw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syfhmrhd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yzqhwpjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdoypahq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3idvpfpoz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qnirchgo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yromcywv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uywigobe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bvitevbv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jxxhbags.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vvjdhmaq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3prexedms.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbgynxyh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjkmtadr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3knexbpts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hwjzixrm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyrhrntm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxwbiqqe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3niqwjsnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zavlirii.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vzlewesw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tizlovmj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tphxzkcy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lhfigjsw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3leiwgylr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gakhimmx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ywpkgxhh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3chfogfnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tknowtef.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3crogwgom.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fujkljjx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qoojnlgq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3agcbzbbg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcbluqol.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvewxvrf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yfglcfli.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypecqkbt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cynaoafq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovwdhosk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3refebywh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ivethcjs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtvtseak.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3reifxqvb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rzjvfttu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sgyslylb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dfryiiel.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3glarcmoj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fidybgqe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zvdtzjjf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fomwtziv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cyaudjcz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ywgtaopt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uklpoyrh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uqsnylbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpxogmvd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3liepvycb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcdnswnm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3btyuvshq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bvjexvam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3soqmoigy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tjqxdkjn.html


<!-- 参考信息 -->