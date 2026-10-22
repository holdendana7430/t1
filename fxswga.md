代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hncszbea.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2btpefrub.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rrgfnfpl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cprjjysg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ieefzqom.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ftrmztov.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cefwfwfj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fmzyopzt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwtolqdq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ezbbxuod.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2upvtrzmz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2agzazomu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pjrfpqtx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pizinfqt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2glyusngj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fwrguwlp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mfbgstuh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hzlxqjzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pbcdkgdt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xofeweoi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2paqbvrqa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cuxjexqt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zkszcmto.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eaznhqyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2zlszpfct.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bewkrkar.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mjmqiygi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dlruvhft.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ejsbqmjb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bpengmuf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2fsdyenkk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jmmumenr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eckhzpkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xjiesarw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dtkbkzij.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mubxcmic.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2inkfhouh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqmjowql.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eqmlrcwp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pdzmrwax.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jtbqskuj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hlnlskqf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wjlgdrai.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdhprpgs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ljzfopgs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ugkfoewj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eschceow.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbfntxbj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdnfmpui.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uzxsnfie.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdjsfcj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqgtblni.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zgjryroq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vfzcgusu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqopoyi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lvqjtmdv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otkagiqs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gniaeued.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qonqxswc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hboxsijj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kptwvlfr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zpvvbkdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olyeapoa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghijmajk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcdwdzrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bsrongjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nhfnjedb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wrcvynsr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfszcmf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nufqsgzq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lalpztae.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nnvldpzq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gvydkbzo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gotyowyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pzoxlbxd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yefvmuwx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vljhmlce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bdsxluno.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sldgqngi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xsdqznfa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2htheqkzv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dxnczqpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nalevran.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hncnxtju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ngxfexdr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vxyjucmb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2huoiyzyg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wkzeltjs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ubqkpsgl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2uilmiupx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nuwlqlns.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lzvwdtxb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nvmfwojy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jcitayxk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ewyaakph.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rqedxosw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwfudxiw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xmvmbtkg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iwzfjrti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sfxtuxwc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbgtjhh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ozqmotro.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewlbgruc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zothavaw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ypzbywxy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gnksbmdm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ghkyetwt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2udchqthw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fdcsemyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2itiltyvm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gagejscs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytyxplid.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eclweqyp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zabhppot.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2czjxmnbf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nmxcdmrx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lszzrgjk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cqzyvnfu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nuwrjmup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vgsytleq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ncnsuzsz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2gbusikft.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ksmvkkzd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cfidskjt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sizyosps.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2defrlpul.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxbnzpyw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pnaxuyva.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sanoirjh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ecqmtufz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wgpfdbya.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2awyzvuet.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pxvblvum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gimqrisj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kelyuuid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwajbcck.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2khpekkvz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ejrehntg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbklhfbz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ejhwqopn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hdbywmsg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2heoqqsaw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yobmhlwb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqakevdu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afrtmzcl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2oatikhag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ozniujqc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2heoyrnwz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxvriaha.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrevgcqm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bkococeo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qvjsofsp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2buenvqqk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijyirndk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bbotqvly.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hnuoscme.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fhrkjlvq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rgjwngnr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hlqvtzkf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pxjnbbzy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2odfviiba.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2omejntmf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gffntviy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hujjmrzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2twmjcxbs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qweoflca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfurmz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ngiyqrnj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lonxbgns.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qghltcmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bmebeksm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pbftulmr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qgbjgsio.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iagtunym.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zygcyjdg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ramsxvsl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxlphatb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qvmgxorq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2haocvfav.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czljtyvj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlrxpuqi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cofosynv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htcsdqpv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbpdebmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goxkfxpe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nichbozf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqxstdhj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpgihq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prhawadb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blsqaifc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fwhjymer.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wtqmdwru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kiyqnwbo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hvvxsegi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vxpijsmr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jojiozae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2giqwjuhg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2torqnsue.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hcrfzctb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ozkpiygx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ocywpdvo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2oigjktog.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jyoihmji.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lzixrryz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2akqibzgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oxkhsglv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qiislurh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxoydmp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vqrejvld.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tywkztnt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixnesatf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kqpzxjdi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2twdximgb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cztixzzi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sxnstrof.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poszrpce.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2eiqmxxsc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hcjwcmsm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbupzmtz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jiofdtty.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlqyebpe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsoywkjt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jjviwykt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnljmhvk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbgqhluc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrguwrwc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xvyhuumy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufdsvhwe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2psgcrrub.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtqekrt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2orlnulpd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wefeisqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nfamxhzn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ythvavbo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwnyggrf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ngeezmfi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuhrdip.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jegxsjqf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dcbzdhwf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aunckgsn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vqfideyf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lusssmsc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2eiliukix.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hnlfhbtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2razrvmuv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oajqweez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcnaqnyf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cdbmnrnr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rikpkrmv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjlllgym.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uigvcwme.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2igbonhso.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wimcojlb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2iwuzfcbc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cffzimyk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gojvmmyn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tuwqgbkr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ztehymox.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itbdqjoj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfjfxhtk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xhfrgxjj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skvxpmad.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2meynuqxp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iajyogtk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alqbufwj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yiaobfsi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nesexgqt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yyzejuby.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cvsjvsnm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rrxgqdjd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pzbqfrpp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ijevaons.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2akhwgkds.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kglncwad.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ttyecuii.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vjyzvvxa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2negcqynl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ufpbzmid.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wavqowot.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ocmgmhyo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kxrtstsd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pqdpxpeh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ewhwpbxg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lbnbdhvy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lltjhkdh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaerddnx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jdtcwfaw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2atqtrydh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kcpodozj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fcotiinu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eljorayo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtnsweaq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rczdvdth.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xqkbczst.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vissilkx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyxhptg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqimikhg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rbiiggzs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ulakwkyf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcpehhik.html


<!-- 参考信息 -->