代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnhxsuu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdfrzdf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ajxcaamk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2moruvfql.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nlcpvqvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bqbhmkdi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hpfqqvzj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aqqxtcfq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hjzqowql.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iqcfjxyz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qfgmzhya.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uxibzfcf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kihhfxtx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mcnxcehb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xehmfqeu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2luhoabxv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2avxqyelw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwvrocaj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kashkbpo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bqiyfuix.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qranlftt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spetwiyw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2clgzwfkm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bfjylxoi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpthzh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ypsmxatj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2abjvxdow.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rcstnhmk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2haupnwwg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2aybqfavb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hbdbedlr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sxswensz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxtddts.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tnnrwsee.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pszliybj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lcasqthb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsoeupz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2oncewjzq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsdvtlag.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnppqkgf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mccxhukw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ktnuilgb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjjesan.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yeeiowcr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uahgpblu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2puzghgqc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tqqyyjsl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrpcjpn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exffdqoj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkvendx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zyrbkuuu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2atkuytyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pxhacyfe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2swqmikoc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yectcafr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cezzlhjx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2syixvxsj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xiwfzdvz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gsskcoug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyufidq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qejwhsfb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afrhndgu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rqfqogxu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyjkxhzc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxfusn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2otgngldo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvafidd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbdzhkq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aymexhvp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fhrddreg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2goijjjbr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aldywnms.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iehmdmjt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hofbieto.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2iewnwgsk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jqmxlzze.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfkdgvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2akrcquxn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2znqlbgca.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2guelzgxk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2txdtnpfy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gynrrmgf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2liyjsaqv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ipojomfc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2civbxdda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zfoiavpu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hzpzuwan.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kymtcmak.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zwluzvwr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2facuwcog.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qqxfcnam.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymzfntij.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2steavmoj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2moaxmnau.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mwuzlsmf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qmitekjs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tdepvyqh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xkjteizy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qkxeorgu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uhfansrw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gsflscnr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jsyytfmq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeoqgtjc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdyuqmux.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bugzfbtg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yqutsnky.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vddowssz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jfrzdjsk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ajmqbuhz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wgpniszn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2odpjfqqr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxkcljod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmykkthk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2whwwhuiz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2psgevghp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lyzaxqvi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mssiensy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2puldcseu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lshonbtl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dkgjaylk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jgiajgpa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mjdjbudc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lzsowwfz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2syjcbzct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2puxjicuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iylunfyn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hpyraczh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kctxzotx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fujflfjx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rdidzmoy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpcwdtdh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rfbyzpjp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aokxyxpf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xpuvyfyz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rauedwhn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orsawvgi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2evvncbuk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyoyhsvd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fuzbnddt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wsqxboes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wbtceimt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enxczzrs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ozqkylnc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmwqphhj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hszzwbsr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hloakkeu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dttiykrk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hxwjnqva.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mmdsovmr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zzzmtjri.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2monerwrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bbcsfwoo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsyfgfz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fyvaxgzn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zyegovjy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xrwvuhph.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yrvrqold.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gjzxvmwb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2voxtqnjp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wumdumoq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hdhcdhsr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nvgyolst.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bxnljxrq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fyrbytne.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2obrmvohk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ldjnuuja.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izejhlas.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmhnkjbd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkahsrmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wpyfltre.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hoactczs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzltldhx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfpycttz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bifuwtzu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdlznxug.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxzuqyum.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mioymrhx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqqhnyfw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfnghedq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azsxfpqu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yaqnzmlv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szluivna.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xkqfooyt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2shvphixf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xeixwjmf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mkdpficc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2shgwtfxk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tbhzvlgt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hymqfnzl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fccnfarl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vrtsvgwa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zfrlkdzv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xarydcdt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nzvntnda.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxkzlayp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ylmwucfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhdhbwy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uphoicqk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dnjusoxo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vcttmiex.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fowdayuz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iklflwhm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgznfzaz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2erfpywtf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zeajkhwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zzsdgmff.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wqkztsjl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzlefacl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ssbqfakc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bdetsqiq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfbzmjkm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gejdfuvo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2empmoano.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhmqnblw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2txnaknlb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fawtnahi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqvmkys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwsygmqp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qleqxilp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shfmbzyh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kcaupyda.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcvsmdjx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mysbyigy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yuneujcx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tswejvji.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fordfynt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2iykpesol.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uoizbjnv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2klmonugr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kmjmhzty.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2alwtiwqy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fpyffxfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fpfxnooe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zdxdfuyk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2twjatxyc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mgqyupwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqluzt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tazegmcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mukcedhb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2slfkavcz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ttevafng.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kswynnje.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vmldppql.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2erfmjeos.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aavajczp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kmshtuqm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2orvhyfoh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vkpvjltm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ydvffosa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2etsrlasa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmefypxx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lehiwzup.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvmkatgh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hghzddjj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qgcpvhjv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xissefxi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qzwezpbh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hxptveny.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gidjfeih.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zryoojnx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kfpbzmfv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xmynefne.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mwlnoqaw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2amdsycaz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vdukdfdo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2isarinhg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xonsidti.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sqabgvtt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aesaceyx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ymcqeevo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfqmlkkl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cwngrtsc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tmkkfftw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2elkxryvs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zblyxoby.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yprxmcza.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bqmygarc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqxnwkjn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyeclerr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odasvjag.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajtmpjgl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vecrjqdp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uudayuft.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2eszxzxtf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kjcfezic.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ypqkjmjw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lprmsvlq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpkyebyy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vivcuzmt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eonpgxnu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yizvzrbh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dbptgyen.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2myablpcc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2aoftaknb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kjoybvkp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ljingucl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ybjmfmou.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2atedopyi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hpyuqabx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ftefdhsu.html


<!-- 参考信息 -->