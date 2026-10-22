代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cabnybrc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jgihsnbn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2calxkuph.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wbfhpyhy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2otfzyjfy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yommexcj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qjgctojz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xqumgrca.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hpqblfri.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqyuji.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uojkvqpr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mqzveqwm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lgcgevyx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ugifqnas.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hwjzaeij.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tzjyzanc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gxvoadsh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2czvtetjr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uxqkpkzt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wqaxbkza.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rwadeyjj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmeawbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pyxqqcmd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wgeihrqd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2menfsttl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gnolbrxe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ywkmksko.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2txmydefa.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zytevcdv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2klvrkrgp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxczdka.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ayjjcznf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wsvjrfrk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztgzqxgp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hcsvylmx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jauidkpp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jslyonoa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sjzxxigl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kjquidnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vqiagxpy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2twanvvgv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ttatmqpz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2flxryrcw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hdaozuqa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wvelvrjm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eenraldf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxxcrlgm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rzpsvbvz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2imnidgcq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zbbsvcfm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lnhecxxd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2edjdvqew.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2waaheupp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwztkemu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcakldob.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubluwjyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xaagcpfn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2blqnupad.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2esyxbhql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gpxwasbl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mznulcku.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ahcxvnwa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cbgtjmya.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qvqlusax.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxeiwbl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jacygqhl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2geycwmzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2oljixnaz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qpvggfoi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zcgwtjfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dvsvxack.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2clpcyuxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gxtlbstt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ueoptfli.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sclijmck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucqwzkyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dbnlmaxb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjrzwfs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eoccejdk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2efwufkrj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bcxkyvyv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xdceiscz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dcqxznns.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tdaifcpl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fxuvvkdv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wpqwsruz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pkycfjgd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fufixynr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ymoniupz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmepujb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uaywhkjp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqhxaqq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qoixqaom.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tulbsmjs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2liydxena.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gwytnrcm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2suvektxw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2muufquxc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rravsrki.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yehnyfgp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2foqzheqe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pemfqcyq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cnxpsjft.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbkxevbb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgbyohjd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tgjnbnfo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rjfiszbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvqguvm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ietmrjim.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzwhdkv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhlanowx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jgisvsvz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2pmbxcmug.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mdmuocot.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2znzfkhok.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vtrzfbsg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fzymkxlx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2svxqimtw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zeisthfd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkvjmixc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmqcseky.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nppoeevc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdyqgand.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fvtooybz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yzrubkdp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mwivqlxh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oruisyik.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bpinkyah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abqcotmo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kbpjlzcj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2izqsylkr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wqhhmvux.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oisyqfgt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwsboubu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pksizudg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vxcywzvg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2suslmyoh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrfzxbc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zydnwrqp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tfaagfal.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nhkbqdbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blpimugc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ukyrgdzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsqpcujr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kbydkthd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mrxvavfz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ykvoiblg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oejzcghw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ogovlixt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2detbrzbx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wffckehx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjrsbfqo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wxlgorse.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vftgeoyp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yuniojyu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcbwrhbw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fywmzftj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2knigbvvc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2juwyxvvi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jtursurx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxxyaui.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wqtrtvir.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ijtytbjt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bqohztel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2holbhvan.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2quakbfmd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vsfhqmbr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2khhestrm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zmentkav.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ornnaftx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rsujcnfa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2isjsjggf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2usqmdwiv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nqcqwahs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wnjknupw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ywozijpm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dbmfbjhf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gjaukrmg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibowwxru.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oedyygjx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2amhdctvn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2oeswqzae.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avrmxqxk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yknmwvmm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fizahuuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vjtrxiuh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mvjwssze.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stvfavwx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xklcfery.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrnnxn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdbsiukn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rcwenpyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ismnbydj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tazjveyx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cuqurhzl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rynxbdpp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghfadkuc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzoczsfx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kxvrjmce.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ofbllpaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sazsekgm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2usgfpeju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qsesqzcw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jhacrngb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nznnxdrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kljpruty.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rtxgdcgn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2phqhirhs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yencrmdf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gewwbcjx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mruiizbq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2okheheel.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2flyqpjjl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pxwawrvo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ldmabnon.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gjhbshqe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ckpdbvgn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmzpxkvw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jzrzanpp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sfcxhgrt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kassglcp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vtglvlrn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nrxpauzg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbzxeijb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2magjuvpk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zjmmbbwj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omkypvnf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vbvoivxt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxwntjal.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rckfinjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2npaokxqq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zelvvtmj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkrweru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znixphsb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzpmfmht.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avcmjlaw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ffpkmcbr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqbgzgje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kphshrkh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nnfukils.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nntwylby.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tspegqim.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mwwgcaoi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bcmcfugw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkhmlxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zymdbnyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pssjjaav.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2auffszcn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2oskvdhay.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2layfcycy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2evuqbpel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tcnqkzor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsmuhhtz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vdcexsjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guhzialp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tphnsfej.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bijlrgko.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2htungegc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujpfdogv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ilxycttz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuvygalz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cackestp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxczazxv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajeugonl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jruhwrwr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2alpbxkhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wlvamuao.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2scjtyuek.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zknlyyra.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jvqtroml.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ldudxclm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gxliismw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kbhhhtxm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gvjrqvqc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fzbcdwxz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ljlsbuly.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wrgiwzum.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xhlrhhnp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yavpphec.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2aixwtjga.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gxejdwmc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yyyqpmbr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uokxztog.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lnjccesu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2upbwnlnm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltpjgmuv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbwppiq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2smczpqfe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vzgqdtkf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pbaijnqs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wukkfpop.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hrqovrju.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yyecujwx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mqjgmtan.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2itrbqjlw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhwegaqe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpegvxbi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tuljllfc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gvjmgqec.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgkgunci.html


<!-- 参考信息 -->