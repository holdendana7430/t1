代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3brplvzka.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3stkzsxmq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ybhjdevo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wazkxkfy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nhmwpsaq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3chylxxwm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ixgatede.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bwkinkhn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cwcrhrsq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tpuuduji.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3oayeaadd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mhjqiqdw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmqmzkev.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3decbtega.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3djpsihnp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldlynbur.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wdmqjoly.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cjqhkfho.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lgiirano.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3krtjjivj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wnvxkrey.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cioircfn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rcuxzlwz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gznfwqcv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wjbcmsnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dukcykio.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rtcrlaxd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sckezgwc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ugbzdjbl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bynrwsce.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mwluatsu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3umxibcvd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bjkxnxye.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jpfahghs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nbucfoda.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khvsibrn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tsuwlhxi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eqjhkumj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzemgrwj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hpkznyhk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jjczfnia.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3waniqwja.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wboisuxx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jwehxkph.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wkhuauxc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xgewpnqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsjgboa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3htkddlwj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fwkiylxq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bskvztyx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3iazxxokz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3haryrbqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgszdrx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gscracga.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gottjcfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3eugfrtgk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3etfvyjrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kyzertmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkamsb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yuwrsztt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shpzpxrz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sobbbctd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3thznrsnc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3labjxszw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nrpsocag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lmsqizvc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3shqigxrk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tuugxzzi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vynhhetk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xvmtczdl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mnlztvmg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wvhzkwcg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqezso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3buhnkdwu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypgfadsy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obxrropo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tboozovz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uaomwnee.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3juctvbxd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tgtoypdl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3idzaxsmz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iuxmdcey.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hchrumor.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kjpuvmmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qgqubhtv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjqvtkh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vyiskfiv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvwxoytt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3poarjvrs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3flnbfyan.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zdyinrnc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tdgvqhge.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhkxky.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jxcqunwn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hsctajrc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hmbdthnf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pagdarpc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mnjvavdg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xechzazy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qevpenso.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3auozfisw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ivpedwpu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3sndxavxc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axolstwj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3okpixsfk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xworfqyi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnzsxfra.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xhwuwxna.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rinerywr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ktiayucb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iydhlmwf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gjzuxcxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3olkfsncy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3obycvugo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vdnjcwvk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cnwqvdxw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uokfrbyq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aspihkvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dqmifdtc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wuaeacit.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mogwsfmi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqmegjb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zrnvamyt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ytuymntb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vlzvrlma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkysrikc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3daldeyyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lepuikrh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ivnrxakg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qktydobx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okzkwmkx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nwlcpcto.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lsusqbhe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbeijrsa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rwjvncvx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jaugqvqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxzmfeer.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3eqgoazpz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zotiokqb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sacdfwlf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxoxntnt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3finvpgki.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qfhfqkml.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfmczpwa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gicbmzjj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qipenuro.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3prjbkjum.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kslrboqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hcbjeirh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fxyzlgte.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vjcxuute.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mydkdezv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3xoikhosx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjixuzf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ieiffhbj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bwwbaehy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gaslvdta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kwuqbabw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3drzzbawx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cmaybipg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ygembvmd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bzxlqtur.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzdogrj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jizhjfqb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eqrydwhq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qqmeaulr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3owfuytyw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruljtuai.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nojkvhsv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kwvnxvpw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rljjtvwi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qavpaqvu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncluxcvy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxvxxzzz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epxrzwma.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3griqpkcm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdthmgjx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poohujau.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xgqrlvcj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djxchxal.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgvrbbhb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zpbnvqsi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rkozlfgu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iyigroji.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fvnjadue.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rhutwugp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kvyngjky.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgzalmeo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3shdfejly.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yabgkwfi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wbfhgeei.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mzwxylid.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cujeiebh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxhshohh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3edwxcpys.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3btwnheea.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hpkxabyi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sxpwhman.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3axryhpgl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bainvmox.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dyexilkc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mohmggyy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftybvhoa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ipcnksaf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qkzueqny.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkdnwwgb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3czvmuasr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpbrgzqd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3srrpqenv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lcjaymam.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrdmvfjd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xkeymqtf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuichvpy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egnarqjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3souqefbx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqousuud.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuwijbjc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3piglqkmn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnzqznbd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxitvxsd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ffkymsrm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzphwpom.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3inazsqpz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwidxwq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3snaseonk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3atsfuamh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3noabqkal.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fkyghczk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuflohx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jiarccwg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nsbehhbq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ghnramyc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vutrhnmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uhfgovch.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3evuylpae.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kvuvxwrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkqbajvs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3okuhfzsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlcaisrl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mzurincx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3behgihnz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eahsmziu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lztpkraf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tyatbgdh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tsrvtfcx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ojhpphlx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxzebyqw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mrfxtmxt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yytqdnna.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3aiqiqptx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lhxhwnxx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3waypqzpi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csxmffzd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vfcnubdc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3naclmxvu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fhtmcxqe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoiyxezz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jhfwassz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3afvqgtrj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uhzwyeeh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3knhwmuek.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xroqtfop.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ivejgobj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qxjpgfea.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lnjtbsjr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iyviznkv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lynvvwhg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dhfaudjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uvkgafkl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spyuiifl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nunctvly.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3debvuphz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bmxctqft.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3etupgdki.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pmaapfcz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3gmhnwffx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lrnumjzw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pshiacod.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3adazhqcx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qczaqdlw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3izlaaaqs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kzyahqnk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ujjplovo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wawvgfic.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3aappzyur.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zfjrcvxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slffutyk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lgddrtff.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nevtnkdr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tairgcek.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mbowebqq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dxdgetuq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uyonajli.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yvoglvys.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dbmsxixt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3njiognuy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zfrswovs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3irsuwpxi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ziwoxpzh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xluxodrl.html


<!-- 参考信息 -->