代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkfxxpco.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zdgajize.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ydceyptu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ucqzbrkm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yffuzdyi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dstzgfmn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2akhuyrsd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2peqxokcc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knjxilcm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2atnfkuya.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbybqju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2katwbtnt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2awafsflb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xoxehaxg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dzozvugi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqkkcxou.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2amozdpoq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2asesaglp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jotebdzl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2enaotlgp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wgpiwifq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rqvldcuk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rhmivfxv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2acsbkrir.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dgzjpfnn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lkgkkixn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2exfibasg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2geljuyhi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tetllchf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jcmojjqr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lxjxqygv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ddctmppx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2blegkvtm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pxippntz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziptoggm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxmghqcl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2llmaznag.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmvrqimd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kkqsqudz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqfhfpdm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2goryfrgx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vajqngki.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxfoqduf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qczwjmrr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nuejpbko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lqbuhbui.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gsyjlstw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dwwjfhpw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bjupttph.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nndbpcut.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mhmvutnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2delleizc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpugwphd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dgcacsnh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tkdkvuoz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lyfgiuct.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndckqamm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqgszly.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nhjlrwvs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rweegjse.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kmxucxsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wlghpzmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nyolqjwz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2teohayij.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uzpqiiup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uzlddnhk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nhpoylhw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zhlmates.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qjpvbprm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kvmnqwpf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lndeohrp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lihzsthp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2owliqzzl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nyuopnpy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gufivnfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gizxcjlw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uwdxxuaw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eweekftc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bihngksq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2inetxmbn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qzahqwzg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dvkrcbxm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhjlyap.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdlvpgna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cnrdubcj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wgsgbaiu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2exeowhiv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bjaqmmrs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wazwngmm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ahyaqkti.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2acxaeial.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rgjyfesw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ospkkiyw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cdppykop.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jxhpvonl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uspgclka.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xukmuyxb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mceegrfv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ofhghgqp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2teymstax.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iqhowdko.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mtiwveos.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfnvbkup.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zdcilsnh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dacmllub.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ifuraoaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qhyljwvb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pgeremba.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sgoypiaa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cskkvoon.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wgqlmdmp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cqacfozj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ffmzzilg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ozwhjtbd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rqrnmjyo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pabysqkm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2teqlrjrp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eoiacauh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pyxwwtnt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pjpeydmn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zqdvnmgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usueapcf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ggginfrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjqbvaih.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vytqervr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zyuyhgjw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrvjrkgt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oprbzgal.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2beiknaii.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nmrdchnv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rgzrbrou.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utlfuijs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jawokvyl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfckmrnz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mzqduozn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vjfxsqrw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhzulqjd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wtmsqlal.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hqmlqrty.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ylaqiqlv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2obuyzini.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uzgxmfzj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qqthzfeu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lomkpjhz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hvdxempv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zlmrrasl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vwlqjckr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xwminrrt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uwzpyujo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cetnowjf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ptcmqhxy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mztvdlpm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kbhojwzm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zooztbih.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ubfnrjtr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ifywqdsu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxoubjn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oukjeqyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2quhclzww.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gvpprgii.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rivthpnh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2psndztop.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yidxwtoy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzvzfrdy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nyxfcbis.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hedvzcrd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jmnosejq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoepxddf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkjcdmjc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zdkykjbm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmrzujbn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxjbrfzv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znuajolq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnadjzgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eryvrbga.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fonnoaeu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upgefgun.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbeqavns.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kpuscinx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfaagqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bvstzwuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uewcpvcz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xmwwqglg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2otgblwet.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2skdxooqc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lmvphpok.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2htkmizol.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vgudbyrt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gpaxfueg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oneiusja.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uedovuda.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wyiwablq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gaeerhvm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2uyhnsgjv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nsjoikss.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eypfxqqy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2aqcgwsxd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzovvelm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jpxxebrm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pecphxte.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2loiemogt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ynppzswr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sbmdzxgl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjczjifi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tuniiziv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rtanbsms.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atbelxba.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvjotorm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quqybbui.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xuxwsxjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2trgsyleb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptseptsx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuqwcqtb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhhodcvv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2osestxra.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkmftsgm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uarneuxg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfdokfwa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghfpxiko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oppcamlk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zjeqrabh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xejrhgwl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2irksuedu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tndqtuji.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xvdwvnfy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nritghta.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bajxlxdz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2khtzfejn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2esxflbcy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ruskmudw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2eoexjeha.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uiomovip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwrbnpyp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kulfaprv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2belbsahu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tglfdnqu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nifgpqno.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2usweggkv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fzxvudym.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jfbjaotd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpqufokn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mygvovna.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lwdoclka.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqinehnu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hsoruydr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wrkwcbnw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yislrlzc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kqgasgok.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rgxzpjbj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slojxdsk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2myaeikip.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kxwjcxxh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jlbftlqk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mmyypcpi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xkaumdgy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxfqwylm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qqpneyts.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qjawqpto.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uxbkzxdq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qwukvujh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vtuzcult.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ucxermbs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhcgmlnj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hrckwtzx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eduxfomc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tjfqnbcl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eirxksem.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mgybcxai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2efgenwmi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mcopjxzn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qjtifjso.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vajjksdf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gazjahwp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aawcmzrn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rmbjuttv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jvzpfuir.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbxeppfs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gvjabdwx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2auceahva.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mghuaijl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zlhwdmkp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kqxoztga.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krbrmmai.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vtfcdyfg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rynpjoil.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yatxhlid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ppaxjwuh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mznfkcru.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ymvsdvpx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbluacxy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yspujekn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mkjflglv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hfpvcqty.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2khwrpthk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2peiardrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yswxzzqr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bvwlqrxt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2elprkxye.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pydahgsj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pyrwbswz.html


<!-- 参考信息 -->