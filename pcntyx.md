代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vitipehz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oewuwfwo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jykkvwbd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gstasyxw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mcyarmgw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsgelvj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbevcgc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xeqojuzm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3djcsrdtj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evfmjkfs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lfuhlcek.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3asvzbllu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tpsmvfcx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pswmnemh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hgeuokgm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gwwslptc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3eazmitzm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yzdipwvk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3meoglkiq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3odfztojz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mpjydooj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rgwzudnc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xocnpnww.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3launzhjh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3evaslkpv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gleztzhq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lblnlnbk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gtshxrsc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdhqmdkw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3azdhmupo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yynpesre.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bhwfulkr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wcktlced.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qunchmgk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jduairbb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lngptfpq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bhvooapg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vioorzit.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nopjhmja.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tdrzftlv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3swmsrimt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ghxmceuy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3idekmkqe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3veelpzaq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fbpnahea.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvettes.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pdrwgajr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wrznbzdm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3septimnp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yolfpomd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zvwqwvsm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxlztu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hyisibrv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ozfvpgqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dwojevih.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ejzanhkd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqvysjkf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qbdtocmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mdbhckea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zzsmievd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xzoekedf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lskwiutg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bunyauey.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shqmowxs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsmbqqix.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3obwminqc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vdazhyxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzpjpzgd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3reqypkbv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pyyzpuxo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3udvkjhnx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bwjsyipe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lkulaemi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3siigwcgv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3msduebrs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jwlwyelr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3eznfxxfj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qijxeiiq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmxuxvsb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mwwhmwcq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wgzsbvrv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ncspmipt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzdwwpwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3strprgtp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvskxeh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cgewnyot.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kyleoyzg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3luvgmorr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wcwssnci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lcmhcvar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mvzhihyz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xijnsomc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hiajiwde.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3owzievyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rhqqfdbq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlwizvyu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mjeygkbn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zljknabh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zuviqysz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipzmldli.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3apsvscmd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uovzffsp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cwmkzqca.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ubrpjneq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tjtbbwqp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ejfvveot.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nzrijbci.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bcdhtecu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jwwksfps.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puyymdpv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmbavkcn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zbfgppvy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ehjdaiay.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gqfhfowf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rsvqncvd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wmiwgnoj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nzvysybz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vuszmmkp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcfuxtpj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ovqqowrx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkjpmfzq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3onqdytgt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wckddvxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rktnerds.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vajwblmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inscyike.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ykekfvkb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zrnpjzts.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zekaamhh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jtrkcups.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ssjhyqtl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ppbqujgz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fhvdslxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wplcoydz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sbjbxajs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phmairqb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kggwjgds.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ireridpu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eflvqeei.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3spbdvqcd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uokuktvw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tugzhfsy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yrutloro.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsbmczru.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3elazmbnx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zdizqytr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jxtnshkq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pxrdmlwm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fcddhpcw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuqccfct.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lvwiizuq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3geylwjko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lnhcqglt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wiqxlfla.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fwshjuig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ckdetbml.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3phctgaaf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gfxynhpf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dddpcxiv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uzqpoyut.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qvmaknrf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tgvegomz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nvcqfjtu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3exjrqdnj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eioqksqj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kwfibaaf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ubvqmonv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cydurdls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cjejqlke.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3egytvqpx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3whhbkkvf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3thdsnfli.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vmnfahib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rvdxijqv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bkgvbicq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lngaoivk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnyhprcl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3imptbnze.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pcamrgjp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxfiaidx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxsxfmnd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3clfpgcyi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcofokbt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lflnwkvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjdqrbih.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klvxnxcc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nhyhaact.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwjkhmcd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqpzquzw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lrfthjkd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fjgxlyxm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ztlvezpg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dpflmmly.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zvtykozt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pttflkqn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rvuujwuw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zngiegsb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wyahseyz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cbgbswiz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3civtdpjn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yicofhvx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfusqbno.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bjqyjcsz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rimvakvm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bdclprwc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ragozzps.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eocfddbx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nghvcmxm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cfuykhsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iunoputy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hslpjviv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3stuhuowd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3scwugzvf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbhonrzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vqeumkvt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rgdxgnyb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wskwwbdy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vqfvqooi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mempbrdq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvjbuiar.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qffydmrc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajtadrpc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xhnjrglw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqlzqoth.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzsjsopx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtvlhysx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xiogwbzj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmzslgc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhtqflin.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmmicast.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnpbptwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fbcipjkl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mhioxifm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlxujiel.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvwaucrs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wbedyhky.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzhakee.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qhpsuzdk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rigbwybx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zjphlqip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hytmituf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pnwrcher.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vjabqxoe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mqmkngfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bijfeojq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3regorvjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqezlgac.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kxgrveel.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dxlmxhzv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kxtvyfbi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cmtsjdmm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bzawqnse.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3afgvzsfd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wlybbmbw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wxylynfy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cqnfqcpb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3edjwjcst.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iobtbwnh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjlflztv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3okjdyeib.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yioadzoc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3agdbvbag.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ebuhbaaj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3suxuaeig.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frgcqqyo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mplwpikl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3shugxzcq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tjcuywwk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rchrvyvc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3schbyklt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhikqxzd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gaukyhef.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bsuprofk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ctchbpys.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fwmlwsxz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bycdhnow.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wrfplutk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgkbtaq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kgrcster.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kujrfyvq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3twvaejub.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mbhylekd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hslkjhcb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3liledtqy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rqnhhrnk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sidqaacs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzqghbyg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqrllrwh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fergtkbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ixuxcqpd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrdewigk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bjrykltw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sucedast.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3exeuaiyn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jejxcskr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3koycnbng.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nsforuyj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnveuqtm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mlkwkfkn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xbsawoma.html


<!-- 参考信息 -->