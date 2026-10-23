代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yliqnnzy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tshykkss.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eenrwtbt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3alsdzpmx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdbulkt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btxlpuyx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rbfpgczc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xznaeckj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bctoljns.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nwaboorh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3eszyfebs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvouqnka.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mscnabqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3brpfglrw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hzwygodo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rbdaybng.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gdszqavc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxkurfm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tgpptupx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bzueeegl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3teruiokg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wxtqzvhg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3plbbedcb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ceihonvh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tqvuvugx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vxygdxke.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rwewiofs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fzvklukb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3aywhnojk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jkwoqvlp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sdkzhgmu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zcgjouuv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cyxpyigm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cqnhzcty.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lacapdpf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hwlzwqki.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pqnwxmam.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3junocqle.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ohtkbrml.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fuvscpvt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qikiffzk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3iesppfnq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kpngkagl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dxvebgin.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhgwchcm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dxvxisvc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hpempqyc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dquvxyhw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qxkvinbb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3btenepoo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dylqzikn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpcdjic.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3omaxhwow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sqschdbx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vqyomygf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fboahpiy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zhpvdmcd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bcrffcaw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eoduxgqz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lmqkxhon.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qondyvmo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3emoilozw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mfxinhje.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3metbsdho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cgcdiekw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xjrvobzo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qwisgeai.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fqbpuvci.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vgugrjow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3logrspbw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gqtxvbke.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3llugzvqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vantiufb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mrogvhgi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hdyhajkz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ivrcbezf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rmdhovvm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymrcnpix.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmsujvx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hszrynds.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pjjiohkj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3uqymnpog.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ovspwuhn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vgnozwdg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tctajmws.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gffbdcfa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xbeltgjs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ztidhtul.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hpyjuwci.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xsgvudhg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtssphnj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zzcdnqcr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxwpdyth.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nzcjkuiu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qjgrljyt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vyfoqrps.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zehbrqjk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdioxa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tyexiqmq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmqgled.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vlkyjqti.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aogpjlla.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wrmhmxci.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tvsnpsaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3flxyzilv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zwgyisxd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3udswfjyc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rizqcrxq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rsbyxsan.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ffnevuaa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwaeoxvr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uacjcxph.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lthlkxvy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xfrttaxf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mbksbdtt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iueidpog.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3geftfzfs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nxgbbxcc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dclqfwvc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ghpqhfes.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3sexceywg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3idqsnlzc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ccsvmjwo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rkwcnaoi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ikgsimmg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nkjpbzso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ixeajlup.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jcvayusz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xzosywhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3briqfvlz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3arywjgcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnmzwhmc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tcrjgzzn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rjvlkugi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhosswss.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nxnuvxqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hjnxkwhm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gwonafra.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3guwnmepm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3psrkegaq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvdezdiy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bjwaxedv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvrokkso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ogdzbeca.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vtbttgns.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdiuycpr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fuekoacr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3voevdjmd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hkpubwwz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzhdqgzc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dutbuauy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tgryqpil.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dhdflnem.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkbvuda.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mcfckrqg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvpycq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sqhexhsl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dhvyrjsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ikntdnxo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wzbstdhj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zgktrpud.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hcbvrype.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jwycnsgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3orkmpxpf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vlyrghhj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yhiaovkv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uxgaauea.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oryfkcbb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3noybofbi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xukdzsvs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ksvyfyxd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxyryjae.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3depppfvg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bgpbxmkb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3veupjdvn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwgafgoj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqnzxyzh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3atxegcaw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yudsqtwt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dftavppb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejqnhitp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbgnamnb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bjurhtga.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbkudxll.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wburhsid.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qgewksdn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qnbozqsn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bhbattyp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nvintbsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ldtawzpn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vvtjxoic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3majcpooj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mznwavwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tfghzmdd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hnltdmvr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kmjbvcnr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uymytjug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3igrnnvvh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3clmmbral.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bkmmuxrk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzrewtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhjavnfl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tuhmctbd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjdjcpyu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3snuhvwpw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohtldoum.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stfjxnyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oluabjsy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hdudaevu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aezdtnmy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3agmfdvzv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iutvtrev.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wmcvvcbm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pstuizsp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwokaine.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3chexzhub.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgtrutvu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpmkoqmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pzjutjth.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oycsuxoi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjqyfvdc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzbbleav.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfajtkwx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iypnayse.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dsmjlfrm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqmlcst.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjnkpiky.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxaoctbw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3trprdcee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzlghvyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ausqxvjr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bkkjlxsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tufdyhkj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zfcdsekh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qoornjuj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zthxjpgg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rjorqlif.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hdgpgxfc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jsjllvja.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vxmfdnwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fujfoziv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3egiecelp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gghgurml.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ysknrtsv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3neqwgyqr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jspbzqks.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzdqzdpy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xogvfamg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3olqewsqj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3akasrimz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uqzotaig.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tixdsaaq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3saixxugd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wvavvboe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gsabynjy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tmkwjjag.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stjhavip.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjnbkix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uwtxuyua.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3owqlibgb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lsbrsdgv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jztloerw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xvpjerfl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zuzhkhci.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3coleqzss.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hgtsfkws.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3josupoif.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3eyaqktln.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gjzlfyga.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ulyezklo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dvfdzcvk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qbilwdtb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zznwuljy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqqfjcb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvmcjepm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nnlvqbzh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwpkiln.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jlbjbmmx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mrfnftge.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mzujrjor.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3geesaiwk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlazvjmt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nntmpgyh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxqndfpg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vqbezauu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3seczcnhl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqotkgjm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usbxyedl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ljvodtnd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jkrggqyd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzyquxg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wxlpsawn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvzzcqc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbvfzuy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rhvtkdbz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bpxzcxpv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kvnlvurv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vxapseun.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3igmazjsb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uosvniov.html


<!-- 参考信息 -->