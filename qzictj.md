代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ckemqoiw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lkfynzsu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2dfkkvoey.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvgyug.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zkawikpw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pcvgldfb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2axdkqwcs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mpqujwhk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fkvjyoxp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xpfcttkd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yqcsxfba.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xallkwaf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2izqzzvkp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2osedlzxj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dqufxqta.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2swqawjhk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jcwvciuq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndepcnet.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hslhynnv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yuwsahvs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zifksdtj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2byjwteio.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wtszansa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tjykfrzn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ociocfnv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uslwkvdb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hkiydnns.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehyuamsw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qruaztbu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rjyngxwt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lqmksbyq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2evbkjmmv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jhhcvpal.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yoenwfza.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dgtbqqdh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2erixcvqr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wiojdrqj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wdeetnuq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xrbnikdp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2itypcfiq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2esmronrh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eyynjcjt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2itocecok.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uyqolmyi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fbrgkmpl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2glzrelnv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fysmudwp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cwfwxiel.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lntgctae.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hebxmyfx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aygxzpru.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aaroctby.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrvjcdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jczmgctq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hkldhwti.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbkbigcc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ypxubnft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2okfkvxsz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hnikeafp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vveknwse.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lmuntbxb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ebevycbc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zfzmfdqk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tgbtrpvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2neimosak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sbkqjmxv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rkxvcjbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbcaxbn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ajqdrbjx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pgqhuhsl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2asvuccid.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnkmznnr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rgqkzfdx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nzyxgjga.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2heuavcyu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gdknqkhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zssqyoce.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2snbpucse.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rjkxoaxk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tdvjzfbn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qwpfbsxw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pmovrtnm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbtpesn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rualgaow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2duxcscxi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mwaqsifd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cmscisto.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bdvehhnq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jgfsltas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkaavcnj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nrezccce.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yubzvqnt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2exqkrfnh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wuhtaihv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvtpry.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bfuydtfy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rapfxyot.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kwaxlnzc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jcbdwkzf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lnliszwa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dgitfwuh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uworlttw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yoijnnpd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nowvrlrv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifhnryqp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nqvtnhpq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rnkxvudx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gyiauofo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sezruenk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kcvwsrnw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xznveksy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hooejabp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bzidgzmr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dinezudc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2esohvmhl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vhmnflhw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ktrsqycw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkzvpwpv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpviqlep.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rcjojunq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jqrmfxef.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2atiupjmz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2orcuvlkj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bnigimmp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tyudrhus.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uyhzgrzi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lvudssfh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2clulyaqn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgzwxrlq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2unqnzzuz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvhqrm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibmwuvzd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxlnocpd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkvghaz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yfzcbpyo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uszalmnu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2flizjkas.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zxufqyra.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2siipotfr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mvhlwctl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gbxvfocp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hygqgkxk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dseezpoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enqbnrhz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdusqkhm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lthixofd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pycyifyl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2grofltku.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kjfmjuil.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qjrlnsbx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lgsaeffz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykigbjqz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hehbnwoy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvtqizuo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2istazuhw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cesdayna.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yigrrons.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grivctiw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2loqcixii.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cspchagt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmbtpvl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2momorhxd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gaayydvw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gfdlkvsz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2raphevni.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cutjqeww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iuldawnf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kqqrqons.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vguvwqsb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zzoerjeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yggjbxqr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2szpsjgma.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kepmwzxz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mllvmtfi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ooinpijh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wgozlevy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cfmnmzoj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwsaxwij.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2plkyjwdr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2enubnkxo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uanpmffn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cjpgcmll.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxzknjrw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdpqxwwi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhuaytkj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gzhrtopy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ppziwwky.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxzzeuqu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efsmtroa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpkruaii.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nylpidjf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkwnovvm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvzvffsz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thzqzqzx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwevdria.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmujewck.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmcltowm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hockrgld.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wrqosscr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ceuokfqi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iddwqatu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ddtcderj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ctlzymiw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nmsqdctt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lslgizrh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2frbvollb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fecbkdyg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uvyeikot.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hsjgpykd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbvttgen.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2loudcopy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lcgllgkl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pplbjumf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xqxwhchn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ejlifvai.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rpkaaesr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mylrcsqz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lprhiabw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mavnkuxk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wpsoairv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2enjkvmap.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjujmzeb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bnubxvhc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbkwcmjg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jrifvbmm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2frrrmhub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgsezjom.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqtuufay.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzmbxskn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqbnnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2piaiwvna.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwgbnhvn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flitddtx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utqtkoqv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xidmahtn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vizjtfos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvmdkfds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dojrkzhj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlfsvibi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxisqqez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2eybifatz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjrldqvc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2igbyxavi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tfvkhkeg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gpyvprcr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zaxnmjqv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2avpbklvx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dzuoklyp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vagmdzna.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zwuhhsli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gbgtvxhq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jootixex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eysqghkp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rbciivcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbbbdrsk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ngdjuwuy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uplepfvl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xxowsutw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2caevjoxy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zudncyzx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfjlryjn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tykdvxrm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eujmklew.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yehtqypq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcqmglle.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qqacviiv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuvvruwe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xzefdqmy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zcahlgrf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlwjtjob.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnzzjgi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyjrnevz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pwjlznvk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ckclpwpl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wzfptalv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sxrsotmv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gxpciudn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qczjuklb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fztoygma.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pubmfpet.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pdqpfsei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lsobdxub.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gdarihxg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2blbftgsq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsirxinf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ckrkxhfm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zukxgmhv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otkbzxbg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lhzbsbkr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2grdmhbid.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2feklyniu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zxguhhue.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tncsewbv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mretdpbw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jesdspei.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xsrwzdrh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qgsribgi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hjkyemgl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gxkjgmdj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yakzxhqp.html


<!-- 参考信息 -->