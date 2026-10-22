代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fgvnipjx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2epmzjzvd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2loljnmcz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2duontddi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tjzuylef.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qosvjadh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ubedalrx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2exmwzjjb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2epxfxqmr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rwidkdiv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jnzobond.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mnakjxcd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aweubjao.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wukqktrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmjawhu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rrdsginn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zfjakrly.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wctaralk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2revqnsnq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ezqxiplg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qcsatjqu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zzsueant.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ycembppg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2liahgwte.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gnnufxot.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueuxpbwu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xdpqcvva.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ajvftpri.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yikpotib.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ukxdfwnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2abpqmxtt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fqulfntq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fopnoiih.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wlyjtdki.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vqflmlkp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qutrhbgt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jehsgjkp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zujkxgav.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqalhhwg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hzsxvlhc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tlkaebhb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2alhkseet.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kewrhixf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bdkxfrsg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qjbluslg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgziheev.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2flibuout.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xpgzbhsx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wepywvxz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xcfzotzp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fuinujso.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mjkynorr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lagjxxnp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lapvxbya.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hiydrlpl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tbhvjvmd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2viigamgh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2brfcldmc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tqnarary.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2igvdmael.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cyfsgkml.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fiwceiub.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bhodscri.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpitjdbv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdbmvm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vzgcundf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ryxdogrs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xvtmyruy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jucvqsfl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmosdrd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zryscsia.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2soqfmbnb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jjnvemlt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2usqituoc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qihposnn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gbkurhja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bgnhssak.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jhsimqth.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dpmwvsrr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zvewleum.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pavkchfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hoiwopuy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twfhneak.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttvgmelx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osfedpqs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hdmcaawe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jldifmnw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtzxaa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecdazhnb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wmxkqpvh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zhleqxnx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hbgehwrh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bhfedjoh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pvgkyjac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zfkekjnd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iydncvhs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dcdnpjfi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2swkpsvyz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tjdcbjnt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rryxlned.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rulxqwoy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pimftimf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqmkgqdd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ohkplqtr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2abjnlyfd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cvafnuge.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2usxkbzdq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xzolkjms.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mkviowcg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggjdldba.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pmcoyfpw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2frjdgvsz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yngvzgbd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fgnfnpyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fxbmempd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vtiucrpi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gzwlxijf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yizjkdox.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yamocehf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lkohpnpp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tfzevojj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xlfgdwfu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lhtisufr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gainroma.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xgqkzdof.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtxbxwi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2emilytiq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hvpikbms.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpvlpddy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pfzvehbj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ggnozxvo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tpnqqpvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zqebflam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vakpeigi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xdptajvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfoslmkg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kvlsnxfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hclfypvz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvjkwpde.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gwlqqmww.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zrqsbash.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kituobgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fgmzglur.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvcdjlj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewoiswno.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxawfnko.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kgpvirwq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2odfplvzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrusqcwb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ugbuednw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdptmyx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zljibqkb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kqmsfblh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2peyhbgbx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mzdklcau.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dvdapgpu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xysvrytk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kruolfmn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rpinqkgg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uimbnryd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eyczwvzu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ziodoazr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sinuwcvr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qtqcxpfc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jocflwjq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zmuczjxa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xohiupxb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2egaflzjf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rultvtzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hpsjcdsp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lfrymnph.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dgqdcozk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nryfnjki.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mqophglo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvyoftzb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxvuomck.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqfvrxvp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndjfxdpg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mjgawtbp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pilypjlu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dteqffwo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nqhthuub.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfaidwle.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gaphmeul.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlfgddmm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vskchbcu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hwqtbmbd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgugttpo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xplsebdi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jaxosxdw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2muhtlhze.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cyhszqax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xnsmlihf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hzaehumf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eqvbxacg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucqexinx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eexgyqsy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2weczkvcl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ocsdkcvf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wguwydtn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tmfgwzxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lpadxkhr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rtnzsgxl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lvrcglcd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lcptofkj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qtckaukl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xnacpgdg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gitnjgso.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tineloea.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rehapfdy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2skiuqnqd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qmwmkuot.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sojstwop.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oqmxtwci.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hqniyavg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ordotbme.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ckgxmnjb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zfeagiot.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhwyiwpz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqyqnnmp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qocyjawf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghlekzsi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2szvyrltq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqvgxjxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbymuvpc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqvoptlv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bapusigh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmplgtvl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zytdbmsz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2djdbexmg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhtwxkyq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tslxnnla.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tdreohhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgyebjuc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uiyohmbf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2temgncxd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzqkskk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zsflklme.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nwiavzkl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fcvogche.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hjhwlzmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2izhpzzop.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fqvvqefa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pwokupao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyvyutju.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cubqidcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjdskwcp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ybfqfmmz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dcqnbaze.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vudrskvi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtfygzlx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2iewnzknu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptudllyk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aivcljew.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pfptaukf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cvwwbslr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2oqwvktmx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2moszgkyp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwytispc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obnzollg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cnasrdcm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umlkmwde.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bdufpcma.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fwqeuheo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxieknql.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ashmzwmo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lbpitbpf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zpxsxijs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ebrdoxyc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2orekepye.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kzhmzegg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xnvribql.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ocxqpqds.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2doitbpza.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ttucjjoi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2etgnwxoh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uvzdqapx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kwqsdyfr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylfdrdvd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xzyuzsvd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ngzhhvbi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2avazkiwe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwypkqro.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kcutdqey.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qbihyffx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tprnusux.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2skuwbupk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2smmyatci.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nnaaeowb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bniupxgl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfnpwk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzgiflot.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2johsnplz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vzvsmcdx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrwfwuda.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yepyoprc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntwdpnll.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sjprbulb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2liihbvkf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzmwgrvi.html


<!-- 参考信息 -->