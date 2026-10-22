代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2corgijsy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zuloqlqh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cyzejkir.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gwoucfkh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dpabnnma.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzspxh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyrzhpv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tcxpviur.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmupnjjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wlupgoez.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2knznblcm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pvgzltpz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2udxlhdxt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tcwbijwp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xummhqqa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzcesdhx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ddixzsfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gojblyyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2oywoqcjd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bwctjuqu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fjekjeim.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jczojcec.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2binqpvws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dlwgeblm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2avkdulpr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fviwgfaj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eyntqguc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ewgqtuzj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqgmlwqo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2luzkcuqb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xeteoade.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bnenfkzp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mnpqthcx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mymylqtw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cdjtzpvp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zelncgic.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aiaramne.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjdxfuam.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrfnrwyp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mowkalcv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2prgjblgm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zwuznxog.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mwfjwvqx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wkhnutqn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2uqlpsmfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjgeenzh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2myjfipox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2riaymrcc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcjvinla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cjesmkev.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ewdlxvzd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2auaimzhz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2oxvagspl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nisbdmhx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2klhrulei.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpsizkh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fsslsmhg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eouoceqa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fxwetwgy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uiyntvth.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bnfnbtdf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nrtgnacc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sujqhbgp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nqnzfrtd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uvuhtgoq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lnikwpmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rokgzzto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejimucqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lvbfklzx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zrdurkmq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ihwpgkbe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ysromjyw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rsagcfbv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqeojvp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ssweiluv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vtpsderg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uiqkujxa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2epuwsjmz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mfhtdqgw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bexyvqox.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcfkie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsggxuvz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cnddafcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yjjremtx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uyghijwd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2esvoptgt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mcxsbgya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2efbbbsjm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mbkqfgcy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qquhavyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mpegbqbq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pvmfykyq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2udabided.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfpigfv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nqubqvvz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2quypoxeq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aewuvzci.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yhgazzns.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rlqrjhhe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qvfbjqvm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnpxuej.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dlltuhks.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftolaaee.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ualdouta.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2llhbnoyw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cltjqyfs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hawftyqi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2shffaptt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mwnryvxm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vcjrdfqt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlueqqnp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cofetvbz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2naqnulnw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nadvryxe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcnxbbou.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2riqtinub.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nhoexwwu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2clbiwwje.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2livluryd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iiwcbgux.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wbllpxre.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2muijjizv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ysjfwgba.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vocprsga.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yvgvfbbv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyafyhmo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tdkfcyrp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rdkfxhdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zocotqfg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zqobupjj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2jbhlrvze.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bpiujrvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wgsukdnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zskgmriz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qofjfwpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piuawwjd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bvelviyh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nynadnvo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2coleetvz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vwmpklyp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rrxzwlif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwrfjuib.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ixyyklse.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdvxdbyz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cywesnlg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2drruroav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tjeotzuk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbxcfge.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2otypggiz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiqneuhc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xsroxhtb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fzllaytb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gcuykjch.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2abarbakt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gwiwyzos.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vhfyozot.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rglubpuz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uuvoiugr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pfmamecc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xkemxlmh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tojmqvcu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tjfijues.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2reltrepd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zuhsyiot.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2feivhise.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xdjlhyik.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jevymgkt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bvfzypen.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jszccdzm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2izmndchy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nszfrylt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kihdmeuy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2porbfzqp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lizmgfik.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygmyqlwp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snpnahwg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgzyyvrv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ljtpcrmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2stmdbaaj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itoikwlu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvpdadyj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aycffzzl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nacnyniq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zevnwlyb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvomtkvz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezcqcpfr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvbnswfu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omfkqtyc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snhxmccd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqcurzsu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gjyolxhq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sqiksjjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2llpsouhk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ztibsmbt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2opawcidf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vbcqsezx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qtzhntfh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2upqmtcbu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lalrloky.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2evclsljs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsvllpr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqznwjqw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqmdfsny.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ssugtvtp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gqsimnqb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gllltgxl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bpfztokz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hibeficv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2clnjgvbe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmydumge.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2plwajjkd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lpmbpwlr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2liliwrzk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gxwqhyox.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dihnzgwk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyibtafs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nohatgtu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2reseljyy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okbiqxtg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yedwhtxx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnxssqrs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frokipxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2owxsgbev.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxdidqm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdunphzs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhnfyooj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xooxavkg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gokpoalc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhphnglb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrcdbqs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbxpmrlw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sprzekqe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xziwzfuo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsdxbwyo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nnzrjevg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rbpvtslq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tjdzavll.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ssqunfto.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2esanttti.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fmanflxm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mmrwnzwu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nhrqmpci.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vnjohtzf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jrjpswaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kddjaocx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2sktxnlny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygdxhuhm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vburhzcp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pjwmkjdo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npgyjbhd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbkiztxp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tiecdgxy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2oppowvag.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sscabhko.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwlgrfkx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kantgpmo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhidqvpw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2szinknjp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onsfoeur.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zacifvnz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wignfwga.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akuwctpz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pvkovkgt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tnbhkcel.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvybtttp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iowminmo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2krfzgnkj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pmdovuvw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qynqdcur.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjmuhdwb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lmirmyph.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ytxjvzhm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jqbjdkbg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2veccrouy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2llkgdnwn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hjtybruh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2extrudsr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wiydatfq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nikhrmdm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djitidgb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqujusr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ewcxahcs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uooqnqsa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dvvpkydp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ljhqdvmf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2niptnzec.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ygqogtwr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bgwoqxxc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhyumauc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uvuavxsr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dwziseyu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlrutyqu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2feayqrwn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xkhpyavr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdxiauqi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pgfbetba.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbngbvp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gmtuwutx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tdjcwybw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oipnlram.html


<!-- 参考信息 -->