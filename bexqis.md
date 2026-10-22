代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2axotikmi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2frxktriy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qevyjdqm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nhsugelh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iwzbabsz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pduantlc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xqozflbw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzoeele.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhhnlgy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2clhxslnw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tvajvmnn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bvswtwhi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bdqzvxgv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ijstoqzu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ecmpcsjf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2shdyhvez.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlxukqcu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ajccnqjo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrfervea.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hpadabsm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bpgnyjdk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vprcqcpa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rfnrqpuv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mjsuofyf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2evvvjaec.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jxfyiiie.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pttrdacv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gwgajhwr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2naaynieb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2atpuuino.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bpznhdyc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ucveebrf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lwjywpxn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iojpovne.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pgivelph.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cblyyjjf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2klzlrrcb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kmyjvuax.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qylyhghz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ocrzmaxt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bgrksuvn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rehvvfmw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jnzcgtyq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2plijgpmf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jyzevelf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lxtbpyds.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbqphuzi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ewtpoxgh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jjbippfg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tggobldp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cusxnpkw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bduskckj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zfixahhm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gudeadnf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ezwelgdd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2srlzemtq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qnujfenj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kucfsgma.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2avvkmqun.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kucflitb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qgvwyhyc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sfkwnafh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cgaynopz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2asionjvq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejubgsgs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2khwmowgv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kgqtbhfz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2evimxtff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ivslyaxf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mpflpjyh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzowozu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qnsvhqcs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhehltm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ineaapko.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yojuecfl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2uhpafztr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2npqnccdw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsflxxe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fgkzmlpo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxrgjd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vhzgzrar.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jstvbfpx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mjsiwpgc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwkwtoq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gyvapzra.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2usgujmbs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2psepcgwk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ouvegxfy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vllhvgvy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ogewckwl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lhzhfvbl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ldnonsie.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tgjwmvsm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dhkempsk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vquxqquf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2veueudtc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbqsczqz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2khpqqlna.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2izwbupfj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yfucyeml.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jdjksudm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjixnfxm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jptgyfqa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oshtjwyk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kcgpdvfk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ydhmiuxl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lrgncbqc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rqxxcelw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rklwtwdv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dxphlhkb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yhyraauu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ttpomhkb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bkrvkmig.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dftsbvju.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2omavzmks.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2irspropp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2waprvcgf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fmlpgwch.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vumzveax.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hypkoood.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsohuqse.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bxvfftgo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2elkmozoe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fyuedvls.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aayuppwy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rhabwqgv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nddahenn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nqlqvnbb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jextihya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rqdychgs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ufahlvkq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzenvtkr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2utgyfwst.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aoixqyyt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ponktdom.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hwctmzcb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vpumnbbj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yytfcwkg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wpdnwnzp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nqzixhbx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2baokjuuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvzoagqe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pnumojfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmiomtbo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cayjiltm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qonhabzs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frlcatza.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lussfwby.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kljnmbuq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zebcluhr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vzjcjwxx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyoulzdf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2isiupxvt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2imoxmvfd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wcbmilry.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdpbzqm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hoifuoyf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2enoimwij.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2luajwcpr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfmmims.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2oljfjhwx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tltyqjlp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wqpiutyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hrkhmnbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2svhwrhkg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yyxpcphw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nqtvjwuy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kpduyzxa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2dvftetii.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2anbzvuok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vfqtoczo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bwtxtfvg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2npztcjkb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2csindkym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2prgigpph.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wykcqmcu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tsvqrjqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gewcrsjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2getgnabm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fheijcwu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gsrdwyyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ykujhzzs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkknarbt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcydjvcp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bezfkkcs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ykcvlpvc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsdmxlz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlfklmjx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vldpthnv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywcctxtf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxnyifxw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbshukqp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2buoktsnt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlcbfqvk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xadascja.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntjgijvt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifksqswf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lpqkhetb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2awaegavd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2erqoowxf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzycbu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2buwnxpqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2luclxweb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwjobkdr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pdllckiq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2slahwwbs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2schgpwcr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cnqdifwh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcetcfbh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zgkqjdrc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gksgxnmb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hajgqgmh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2htwmkiqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhelwcii.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2munemqio.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hlzplnfb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bmtpaeir.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkgcyfnr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhbqgyla.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tudxpknr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ruomffgx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvvsqrfb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2opxrixsx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2csiispqo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uwmesonl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ogckxsti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kimwenbs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agvyigwp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffuwuuqd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtzkqpoj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xzbszjsj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2medcpjrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avnuflhl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwpogstc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mmafpyuo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbcungtd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zrnedxvw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfgujcxw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtpofxsn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jpgopwjp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pymywajm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjdohrnb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yandohtw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vznwuksn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ncazlgtv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2thlanxhq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uawxhrgu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vaxzlyqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bwavidnz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mfdxqdnr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pobwblna.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vyykhsmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbngkypo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qebpgybe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbktlnof.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qgcyphgm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2helxfqzd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zzzarwzv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iblytoqn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sparbzit.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2isxwrldu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nbpjkthd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ugsnqobx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzuqarte.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jbvabghm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2eobokoro.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2sanqwlmd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwtqdqav.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylsijefy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ropkowpp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbsoxmq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2exqqdndg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ekbqmoyz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dzeexker.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vqdrvchj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fmobuqfw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zpooicst.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2osubzihe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2psilndup.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zsisjnnn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zjxmgfml.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xunvflfg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hergpexc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2duwrgytx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rccgtmgo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2srzcdzzl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmezyhb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjynwbux.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ueqdhuxr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tsocawqu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ncdjjkxp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cwfaawne.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2azogfsrm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yolhivdh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbzxgjjn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mduiqamt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yadebjdj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hnnevukk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2frmriaya.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfyqdptp.html


<!-- 参考信息 -->