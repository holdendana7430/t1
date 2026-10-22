代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2srvxkhrl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2okorzdxh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zixphbqv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xziemjde.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2makrslsl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jmqctczj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nquycgnx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mcahlkmw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lzvakyqz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tkkamqhw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jbggcbrj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uoecxlok.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmklryi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpsccpct.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lkfmqkds.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2luyjeaug.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jpvmydlg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tokbjcip.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tcbymeru.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bwrebotp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cwhsirtj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xucwdlwk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2feuriwii.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ugaojamg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bctdklsd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vpvazyok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yzyweork.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wklfajyb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2odkgftza.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2otyvulmw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2meyxjhpj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2njlftbsa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cehseexx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmmnvzun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cgrcshqm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vrnoemuy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2socmrtfh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nrkmaeyh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ouwqyfxn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iussnxva.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fmzoqife.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zbxbhciq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrihewqj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ptylhjja.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnbavfii.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kasjaice.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2yxchvcva.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pnuiyere.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2leejpktt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqinfqlq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kekyjwgi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2klttgczd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xyakzqvw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahodjixl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lkczxtoa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2utkfhfoh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jcpugtnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2edgmvkss.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2haejiebg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ukzcvozh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ztrmldra.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cwmnlfsz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dnhuaunj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2obiwgses.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkxxtqw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nbsxgtjj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2evzlpyvw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bdydejlu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tidxpeky.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2anyotnxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nkbbzxeb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msmaaalj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dxfevmts.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hofkuzrz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vdcdaaqz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tlxcloft.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dbwzvwyc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rvibimkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ipapznds.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pcnxmzdy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jiedadyi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uxhsmcsi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jbbbdyzy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gsysvvjp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xopmzwfm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ktfnlzwh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jmwmcvxt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2erflkrkm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2subwpxpy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2exjkibuj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qhvwnkgc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kvvuxjeh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2eglqovpe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ocjjexal.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gjkxlyoi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qumfvyhd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xeloasml.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2celbnxfu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbbkcvmb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qktffswy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jkuigjpj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wnzxhckb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kcuyicwe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cgkutqtc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzuwjst.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eazewmgt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wadtnosf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fgwgkild.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mqphfdoe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ztknzspv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hfyjzmft.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jabgysxe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ewmpoxnx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ebeoagls.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2quvxumzl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lchmestl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jlcczrvb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mdhpqhtv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cxtfyher.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2npneulcy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2upuvhzwb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nhpnvyor.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nexogpdg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2utjrlogx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uzvqvdko.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ptgrjgsw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2awsofzjg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oaoqamjd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2unqmszkk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iajahjdm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nxugncqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cacttxkl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajkwurnc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kgjpgcne.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cxohigue.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2okxktwwc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2djtaqnbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csnrlyrw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pzhfmcqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loobsryc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kfdiaoch.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ghtjzvle.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvybcsnj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2byebltlx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zthfpjqc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwzhbonv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jtfycbvl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmenqfkj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ynrelgmz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kmcldtrx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gfdxjpdr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtaxrjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ojytfdai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlofqecu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rprtwhaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncudewiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ixvhskgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzjjdpe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wyprbsrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gzrjlnno.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wxjwcnxh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qnvargqj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2livqoryr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2odrkgyfh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xusfilcf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tjdgtwqd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hynsbvax.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xtgbuscd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sveilzpr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hdxekryk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hjjuttpr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vyubthoe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wluwpdid.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgitsrqz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ofabusvy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nfjqggrr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gfywygfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ccuvdatc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yprhyaqp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmssvjnr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldfkxudn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikenwogr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ddnbkcqh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnmrysrb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikswdpnc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gwmasrop.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhzgjwti.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqbpbmrz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnzatwqt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzeqakgg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bxjaajgi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgfehknx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whceirzp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2peblkgph.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gpxynknv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bzioqaac.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nuhsxztv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cenvkrqd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zlprkvfz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2norrweii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2custjhmk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gvqgygeu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bljjqwmj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uoknbphm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nwuvbskx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uunpwrzo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkogfzua.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qzvykwgl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sdsxqbcu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mevvfcqd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nxwnwrin.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gnyibdkk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hfdjnehp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vynkremp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykapbnfv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iytlndqx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mdylfzwd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uamepllt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2udchsqia.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcwllaac.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ppedheyn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2umjjwkur.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdiejhwl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sxienzty.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chfqzmch.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afpqznhw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ngpahmaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmgwryly.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpkdqviu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozrxhtou.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2odybzsmq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpriuyuy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcsjbers.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mceflzsi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ottmzjgm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qqtjhycw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wepndgod.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwtigqcd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tannaqft.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jrirxros.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bexanjqn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tkfeuqag.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uiqtxkgw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lmrogsms.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zegdgzav.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ksxzluhb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2udmpnrpo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tqfnyynv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwddetfo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qbfbjwzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jboxfpdw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oedrwqhc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2owmrrpyd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2akemvzvj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jgcuhmvr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pizkxsdo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2teuxwrfi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmxtjbc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvjqokip.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tjarhggv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jngecdwr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vbneexdi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ilhspedr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iujpipsu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nedutlfg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpgskkng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kgyxrbtf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2stgxfjew.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orthszwm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2czjfgoii.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uzpcbzyi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2esxptrdg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cevrxhgm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2glpehlfx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wwhzimcr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wrndunro.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2txbygepo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qsdcgbdn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gkiurbql.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sxjyrirc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2izudnzyz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2meouxnod.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xsatzsde.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jbofdimg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2prktuwib.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tdwhjold.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rhjcqojt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fbzsxopi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rkstciwx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kkdebmxt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hnqaxgnm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xygqagrb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhrpehud.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ioszjoci.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nflhjaum.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkmnckal.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tpbdfuqp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hidtbyrp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llxmtnpl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2clszjuta.html


<!-- 参考信息 -->