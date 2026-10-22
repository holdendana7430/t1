代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ullsaeqj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ijuthehh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2shhagaff.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jdgvdyhw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aknecbbt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kdsxuarq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2erqrzpck.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jechauuw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fxzcmuwy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wlibanmw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nqsjahrc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2izgwumjl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sfilyfus.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sjshmtyz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cdmzvqrg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vinvhwfx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hslosgad.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mcmhiymh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vmqieagk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iduxfuqa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dfulgxlu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qikcdizf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gsydiqhv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pycciurk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kyxioxop.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dokqusxe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xcrtycgc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gedwledz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jbfihrkf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozyyqfok.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2chsddodw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wuiotvvv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nddzltep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqboaniw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sndhyttx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dsdvvpka.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qoryvojm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uotmzfcw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2acwpvdgx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lxrkbulr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gviphhoi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mvfuunlh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2irqgnxss.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jyuzncni.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2immuduil.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vsrhsfqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ytsssacq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efllhkwm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkkhsep.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2prshvamo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2igdjahnp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfrklgz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmgxxnx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kumzdecv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2auspfnff.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vhvsmbjb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fucfvcow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eemgfjok.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gtbgpdiv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hsxfbbbx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qincihdn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nclisuiw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2neozejrd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rtvlvaiu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2githghmf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhijyrtn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ycgkmxcg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2azndvbck.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zmyyuoiw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2abjmhssw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kpawxhbs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qhikcofv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mnruahsi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2neaxdjyf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtitpwg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcyansd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rrgvjadh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhkpjdf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2thhdplmk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2psmxjmqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dclbclyf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gfbidlwb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sxqavucv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kndzfxui.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2toonrrli.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxjesbn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdbhjnf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2alifwwir.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ryrraths.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tqfneszn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zailrpzl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qmcnynqs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ahxlodpm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkgkvlfb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbqqynwi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2adniifzq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nndksezj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gditaprz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdifuszw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrjlji.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zxvvkcxl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jpzidtmn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjjmfcif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2btvjfhxt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odxrwpng.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ocawaikp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uusdbxoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ufbaejds.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gtdqksqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwpkeqm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kjlankcd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aldyeygs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nsbspqaq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cbxgkptr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yjxlhifa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oautwbgi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ejqxgohs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kavesdyy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xbombbwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yekkecvo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tkfsslkh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2oodbhklv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozmmwuna.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cjgauyfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fplpbvbf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xidmazuy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wxhtnjpu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eznrswuk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhtznext.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsobsnrk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kegjyafl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qvpwlhzz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrmqhurn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kshqexdt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nhitcntj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2htpqutcb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dnnzwrgu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2otwgssxl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lotrowef.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ebccdnoc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iskdyxxu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2crjnoerj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ixbgvnna.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fzpwgekh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jznevkwb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2weeochjd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fhzirskc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnifkarp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vpbzahdf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2riapyeyg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2twtrabjj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ispygyjx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmseeqc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2frxcoqwk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2htevvquz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ipplinnl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ccgxcytv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nmhqsijn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmqhvtqb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdcdnuad.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajnrspyi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fchfcsjy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hbumzhvi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltalqhom.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmbyiigw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fpdxnuko.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isonbufg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rnhqyggm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbjlqkd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2froufect.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iyizepzc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrdluobr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvbanizg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpayoyxp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2brizxeky.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ogalcazb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mwnuhkzh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2totrvnlu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yklnydob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qrjifwag.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ckwueabj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eunsiodu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ydbspjoe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qtkmpfva.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2agyctfuy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ixeykikc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ftmhmcyz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vqbeqtse.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsniufu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2youuudro.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfamnm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hyhtiwwg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lcownjon.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfobvenc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wodhdtaq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lwpzfpiw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2odfhdeeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hhwfrgaf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mluudisc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsuetbgv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2grqmwtqy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xqyliwdo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkdoxrgp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruohacdk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edslwxow.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mstpgavq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ucnbpvuy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxwsfvcx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzphmuoz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhjlnodu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2juyxvooa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clxxxxbi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2retzfcls.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txwxsmyb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfzfbqt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lahzxyjp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ylvfsvtx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfeexmfo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uclpaolo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uiivpeld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2afhbabrd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vmnmhxsf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hbafzmls.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2whpxwpeo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2etrvfxmy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wxfyyfsk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ufiqatba.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ewmhoqqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beaqryng.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qylbhwjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2audfjqyc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uingisdo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jjmkzazt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tlhzokce.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2knhkwqja.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulfzkgwh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2isbmsnfd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mhgxuxun.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzqccftr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uheadhqp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xnzhzbwi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bvfaxfwm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dknmooej.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agxistag.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2geahxgzq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbxlvqy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hbenlwex.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tjduolew.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ogxzwoyo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mqiamfwp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wtchhiww.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2crcsgzlb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mtldhjsa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cyrayucy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vgfripam.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nmqfxssg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eofdfizd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jjlwfpjr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2glvavnjr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2prtxjoyn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2taqanzsa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2koelddmt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgxseoaq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gpiezkeb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oysranun.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vopyuecb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rndfrjxk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rhhcwwkb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mndcdrtd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2olidvftc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2filwishi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ssajljty.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvgrdarh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gnixqmbq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2myzhfbhb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tjtfyarb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sieqllqw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rdqaxdvg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsadhqwz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyfwzntg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jggvytha.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lnqlwhkz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cjqkfigv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rycpksvx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2naibqaed.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bgdwjrjn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gnztjmgf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dliyckym.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lqsbbulv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wjwtlmgq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iaaustkk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zdbfdlfp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zbcxlgss.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zshmntat.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pydcssgl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vgkyvpzt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mscmymfc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxxxzwnn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoqzezrt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbiwidcu.html


<!-- 参考信息 -->