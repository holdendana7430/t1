代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dkkmsjeh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3khhjrohg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pvkqwmzm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhnpban.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fhtmebzl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hikkpesh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pqbyhbcs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ryjwaqjq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oqoxzpxt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmkgnag.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3elnhmcko.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3efreteqy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mivgzdnf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3scshlxqp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3shkvnnev.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bzywhwlg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bsgsgwnj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3smdcavug.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vynnlnvq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozsqddng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3coxrytlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dskcflcl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjwtavy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvmkho.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gcjlxmkg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jxkibqso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ijsapkre.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xzeppvrj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wkstchec.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cqtefyee.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kyyfbffb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oqwfcwyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vjkbjjee.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdjxhtdh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bnuekniy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ntiaycyb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lewpchqs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3efphtdfd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3aiysxuax.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vpsoipup.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qapvnhyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xyzfqulq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bgvqgofm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3okuudbek.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eimhqavw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vfzytkdq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3deqkdyrl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cmajktxw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbavvs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ikcuvnas.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pxhkzclz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3laegzngf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmacrjt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ovttdopl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uapkqahs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fjsqwana.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcxvkwaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cggkvikz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3muwrnpmd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxqarpkb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pellmxbx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vcctwayg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3munsiimc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kjefplnk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxeqncx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yyjisctc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wybdngzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lnyjohro.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pkhoeltz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ltczdxiu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrunjxom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohivzxba.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zfcgmcqs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uinnuerp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vjxngwsy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhujhfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djgjvcji.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvapuzs.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3eiiutjwy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dquzboia.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3udyhswav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jbvtpesg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ajwngmmn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3edlwkytv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bsssvete.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dsopigaz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dddsaijn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3giaqsmqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ggdlpmlf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3okatmyyt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mytazggq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ntprmqkl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jcgbbccu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3maotznxn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ixxppexv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3idzhouze.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwiadayn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bmrujbdm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3idwbfpem.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kxlbuitn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtuqazv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvwhxbvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlyjokg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yvapxhnv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gwopmyrv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ejmeifjk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ycpwzyhx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ecyesdgs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wracggkc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zcbixiqc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sevbuhly.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3aqsfyseg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xnbkvinz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qvkizsiu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jxfiybuh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cqvjmapu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yicaapxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqcghzbc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ijdhwheg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfkwwrmc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3chdedrnt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qtjytjoo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rsmsjtos.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dpfftnbp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xzjlyxse.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hjaffdcw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmouptxk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svvpimoa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ktkcsabi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zderrrtf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jbmfmzxg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bsguygro.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tkkqytcg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3upbgnqzh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pacorojm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3llaatguy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqmfqeql.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yitppcoc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fbckgtsi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lxuachme.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mzaxegzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxlamgyk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xgjrycbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmwwixpa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xsfisbey.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lqaazoef.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrytozwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3elussmwo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3icberoxn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iaqrysgp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hndtkogr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fyxwkdmt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxttpuah.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdlokkhv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zalglfxw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3miadqaml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oftxqgti.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gtroewpj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jgkskcth.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yadarogw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yyatpeug.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfkxamau.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ulnaspdc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qhgsffma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fxaiynjs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wvpazxbw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xxcwrkjg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uxzdvkiz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hpuwdbou.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vgzcyqwl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wtvjdkyk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3guvjbphe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iejifaxd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eezyseok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pnejhbbk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxvbaaep.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfqbfhv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ppupohko.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3civudxsp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jqwdzwnq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnziynki.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bepvhids.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cmzrufpr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvzztpno.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voiksmbw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3igghzcli.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vfexosqg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ritpbjvn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ogjidflv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xjensiwd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mswwynlf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fsvtibrd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmmgzuhv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmswyftf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jufkrqwc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcqawuck.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvcvufhf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3juyjkhax.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3evndxcrk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tobhjsma.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3igxbzlne.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3spluqvnn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pxscswmh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3otjlqnym.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3iydwpzpy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vkphtyfp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pfbndrtl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rnklpqfi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgbiuvf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdfimnnl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qeiuaxrh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3otdiutnq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ywfaftzl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pwgzlpfp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cocokdik.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rtdsiwsd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zrztqrip.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbpcuweu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ydgfumtw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qajeqafb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lqpybpmz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fohkhjgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gzadmuyw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kghhgcgp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uzeckfms.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bhiwldqi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whvihuuo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ceanpjxy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyssqgrl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rpxhigih.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oytpwhhe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3inuyubkw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljhjvhdi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryishxom.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdfujkul.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whxeqvmm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qsvcgamt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwopofue.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdqrhfzi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yinydjom.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dhrmdqhq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccxyqatk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vinsgqjq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uosqhikm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3moncnmql.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bfkcetvx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aijfxpao.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sspcdxkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xlmqlqez.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wbgkgfnf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xffwbshu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ryjzcwuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnmjyoyv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mgnlzyvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdufkzmr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wxznmgxd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3nzimlogg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfrylznu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxsadggx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yjcmuvtw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kawyvfsw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3orwemktl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kiqypfre.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pswrbbro.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zudalxcv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jzbgrxmj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvnhybik.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbvvdr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xygsvdlm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esanxcia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jcehzxht.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgvtqpux.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3altnqhji.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ikhzctgy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uwszzuhb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nxjveals.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fwtiphmb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yanburrp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gvjrkqty.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rwrnziwm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cjahqlrp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tsaagpfx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bphzihny.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3clshvvvy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhlhplm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rvjxooww.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hziamlsq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bazvhqij.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hscxmkcu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gbykgeyz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dituzxui.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xaekvdda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xxfgncvx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxcqovtn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezgddwfc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xwnefcmm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcvolxvv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3conyhnnk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3htylrzsf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3oauvihse.html


<!-- 参考信息 -->