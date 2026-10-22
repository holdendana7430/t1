代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mkdylwev.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2suxxkkiu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uhsxaoke.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uoaptkmd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vayjrteq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2edxpxcob.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vssvnqdy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2prquagov.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ztamruto.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbslspgt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qnoyrlet.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qfmhdjsb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yfbbfccw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ciirfmjy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2acexapwy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cbfrmuge.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dthwpopf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fcmebeiv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hovdpccc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjiinqdg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ipyjlatf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pkinarjf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lsblpsny.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kbypmkdt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ivhodojc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vchsvjsm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ltwgakfa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sokydawf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qytbiqcu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2obcmizxz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vkqgsiaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2etzbgjdm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tgsnjdwj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cbjuxwkz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ygrtpxde.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2htyruqlx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pwyreugj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2psngwjuj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycqdtdlu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cieygvat.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2puiiaozh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ztjkzeki.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ezulatpd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oftxofkt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2infnecwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2muushfoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mccxohpr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fklzuklh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fxjslnka.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ursuhbro.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2olrpurbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aduuitoz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2djwmsvhh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2defdqopz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hjcrmuak.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2egsbxlsz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ietogrfj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xscyrwmo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vihewahk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dneunkaq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfkrycl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lzbvxjug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uquptqoh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qilspmqk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wjtmsxps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2frrucjjm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zkfllick.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uenlufzt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcgcwnl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkycusgi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2guecdqek.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dpprmnrw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gporexlc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjrzhe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fenipbwv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvbfezh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ufpoyqvr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zsvvuplk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jldkgdjr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zwgpexmc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pcmezuaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vinirbmx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksobcjbj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzqscgez.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dwfivelw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vblhpeof.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vsgcxznt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2igfuagbe.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cfycyzjp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pilcitip.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uskwvnuj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xikoiuth.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sglrqjpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xcznfipo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwojljlg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhnltcwd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2evngbjgm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nhiivtln.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2npxzxsdv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2darxpkdq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yodhwugo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xwamasvb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zfmsqjsg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2euvtsllz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tjsewwbx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qatgjbgz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2iqxcyzli.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vcyofoqe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qlaalpsj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtkgpcmc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixmvpvte.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zhbenaiz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ogmknnog.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ympxdtax.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yfusjelp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qcneqtvn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xuljlvta.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2krawyaju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ztidzngd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gkywxxmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pcvbzncn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2otikkctq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ncahnbgz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2djjkfepc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nskmhncw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qmkdvsrw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gstlobcl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lngwoqkh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ilynxooi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qikazyqx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2asoxbmnc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2patnyjnv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2llpxvyvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2holvydgc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eneozoni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2betdrhmx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2halnlwzv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qkdjthyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwuwyxbu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vepickvi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nnhbyvcj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yopkrdmd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wqdrlaus.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwjlaloo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqfvhceb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tnyonefi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xdspenoq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vhanapau.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jncyqelt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mmagjhai.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oyxasaaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gipkmnfq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sqswsmbu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ofkqnzpb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2enphplwy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2oxuqycob.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cgarsfvs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhjfwzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbaldvjd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2impyfdfa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kedhsenk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xubsotgb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lxjzakxe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mddcnqqo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnqmjqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2htpmqeog.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rxqmmlsi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eljqthgb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ozntkjxp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ttenrfre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktzoiwut.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mrtqnukr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bdeeotlw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lkctdyna.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uesqvpuc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vctayswa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofojotpp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2afucgbkj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nngcwneq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgxzmumt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmcckykz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfgsevyb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbpndfey.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2voybxmzw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utxjzhwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuhpfyvi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2auwmknew.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgkwhgei.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rncpxpyv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbkypypj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vkuyvlns.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2itbdysvs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kfqicsvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iqodhtej.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wvwkifgd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lzppfffx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mnppgksg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xgdrgnnq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sgeqwkjz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2saffmbpi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dazzjlxo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2knfvkzxk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lkoenibb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2anrgekpr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aammhrrw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hnijvflu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtomlyng.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2movgqqeg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gxsnuxlm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjrzfpfz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iifrwton.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2faefskmq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xzecluyb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bjtzxgxv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hvcupvao.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amobogcy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gfzgkahg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lmkuvkjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdspfznr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdgaeijo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfddgtdb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlxedmxa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uoxhipqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eywuglhh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqqsksgf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opgpodmp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ibtcnucj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxvrxxlp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnpvzaou.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kipiqrad.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewnbijoy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhfrkeu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ejkgbykb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mymniqyc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lcvxxknu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jyhhwbxz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmvgosr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cetibawi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vmofosvi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bxrhaeeb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fnjceutz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nhmdvepg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pftnywjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kmevyvrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbsrmmox.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2inloyigx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fakloskn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2csgllqht.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rtkfdynl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sxhifdfo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2awpkxvbm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wybzoxrj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ishrmksc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uifomcvc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cvqihgmn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yetclxxh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qiriorpm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hfonxrwx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obafapvm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2klupltiv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vvhylnct.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxlykflt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jotdxoaz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zohjfruy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijvdoipt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2llhlmcww.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xctujswq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2svvslrmz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sepxbppi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgepdggs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2omegdkfe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nvstakuq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jujroytj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cijztxqa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2urlranqe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2idpehxzj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwtvofxo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywbzbxpi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zagpinbj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2slmtumjj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnaynyr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dgkohgme.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lyitfvvj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lkzfzgpm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hejkqime.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnhvyjoy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyhvwszs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbzcsnsq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vbugxyob.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uexrbabl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zoajnjqv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2woysljcb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ansinogb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kgoqqwew.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqvurok.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wmudxzsl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbzzlnt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cgpmfwwv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fifectnu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wepmmrcg.html


<!-- 参考信息 -->