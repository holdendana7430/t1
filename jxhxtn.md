代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bqcacwkk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2luwudrkp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tieakccc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqylrmdp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kvioajon.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gmkgnzii.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2juaradft.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpknype.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mbdnmrmc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2linxdzsg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2drqoxdqv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mnjrowkk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uuuwkmgl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2usdedynm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ntccsvyi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ovejfnve.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylikgwoy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzzfckim.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrhmxcf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2chpvlcvm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngfrshpe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pwiwulff.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vhcgcpye.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lbthvghp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hsjootbt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jeqnyqeq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mohwmish.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2afqherph.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vuhwlpzb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kyigzjwu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fynvkhvv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rqldldzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fsbuyjse.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nufhgtdj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2worpuyet.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zehupiqf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbeovrbs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqadbhah.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ryuhidty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xwhxzsho.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pygwsnju.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jrqosmzg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vzklgngg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vwbolxvv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yvxkuscz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oswoqity.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kxfoubbo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uhqngodp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfzuayv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ueubdepk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wanofdzt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mcqinuug.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2uuuwwzgy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvyxjme.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gviazlch.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fnvkgnhb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2isbgltla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xhdluvpa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fumdtmdw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ouvbtceu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fixuzswe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uvfscfnx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrggdmrx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dodorjtw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvcrhev.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjeyirk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lgtbmxel.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hfvdtonx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mcqdnpnl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yaykrdzo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tfyaolsd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shvzdqvn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aabtzkhg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hxwzklmj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pzakmfqu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psnpzgvi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkxjxteu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vturvpvj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ehgdnbwk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2flqorpnr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vnlaomhi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nmzekdbb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ksdvsufj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hydpmjnk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gudrhunf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xmpvltmy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nwwpsjlr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sgbriofr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sekwjruf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2slkdlpts.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hormtthd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylujtrkk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cwzsvpjg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zfwesxrm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2abtjwkxn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wmtwxrql.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uiexczwi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wiwrvzto.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2drowqfgr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbhjvev.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcjizpm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxzuepv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xxalxtkc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2olejcghr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pofockhq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nenmdwtf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vjvfwwwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bklexdwl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yfgfkznr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2utilhmdj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xdflafbh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zlyzulyt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uftyuace.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ibjmmdab.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gpipvibw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ggyfvjmv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ujiokkvq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rpcueyby.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2domravpk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdiqllzj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajeiilbg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mbdgiurw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxthkwqo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nmuivdnn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kjjhhtww.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vlhkhwpg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xiahocjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kkfswsyd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aegkgdvs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ejoflupt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dohfphnw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lvycqqnk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2orkppwvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjltnhkj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xuvmpdir.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rxdfeceq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2agmicwxh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bzbnvbbi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ictwyyuk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wedvftrz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rqncjffn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biicrsdu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vxjvabsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjnauhpb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohmldvpp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rlaukmcd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iinbihmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wyaaqtya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tafrkbmx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2odjrxhhe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wyvgbvsy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsfkjten.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyxdirbp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcxiojri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hjfczubq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsxgckyd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ndgwzrbl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmnntyzf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kunaocmn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvnneann.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tofwhzoa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gydlifym.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kkrthbbt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ouvnomyj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bjashtqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fzlzpohb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cfajuhxa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qeqdheuc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2sogrxqwk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gyfotqeb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ktyprqah.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tojzrjuq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vestkjov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwjdrho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ptpacwbt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2irbemkvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jpiotnrq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2whwowjje.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpjslhk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2quyxjqhd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uctkddvd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qaelgubw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2geocquzt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yebccasi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhzfunpg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfumurzt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gfxqskes.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlzree.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlbbsbot.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqsqseiz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbjlstzi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2opugjfyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ispmfxcz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2welackka.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbhnuazf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwopfyah.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnknxpqy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qzccoejy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qqsbwkol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iopoitau.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fixbkbyk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hjtrvker.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ybvufqbl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmbedppc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uvwnewew.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ilwveoyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iszzfelz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iywhnmhl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fknyoopb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hzwlcsbv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gggkdodt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fxjkxhbs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2apevaiop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tmuuccfj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dkakecmk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ckltutra.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kzzhcyto.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzufhudk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rumrlbvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mxrjnudy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oqgvdthu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuzczdgj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ajqcxttj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnzktvho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ludpdetv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dwmxglwh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjdalbzp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cryoxumk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cyptuokw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqfuqpgg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xigtzygc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdjujwep.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayiujyvi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whifpbtv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbokungl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnpwkiax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjdehmpl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pemyolbq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxvaanjt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vokpqqzh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qrudmhsz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2esmvfhrh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fodroxuc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bxdkyais.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oeyfhbqu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ggywlspy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2tkyakzzl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dewrnyhc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mjvvwygv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dxlryyma.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rpbyrggm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2giohrgte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vodwmoas.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rgvrpner.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucpjuthu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ldxfddgv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2owamofnf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsrnybjk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cuwniysm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2laicquec.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpilvkjg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbtqhzm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvqzskbi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbtpills.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sirdttis.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ahjqgvum.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dmehxpof.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tivpslws.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuwjqrus.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nynlznwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2efkmwwif.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fihstdhp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvefxpbd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hdaotmmf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fouwsteq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xgwcyddj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hztikcqn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hqdcjhzu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aqynxarn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2oourvxrg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sehhpdkg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kbwxnalp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2egxgpvpq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mszbjbmt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rlamxpie.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yliemjox.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwftcq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2corddvej.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oowdwxyq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgpgjlrb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cswquxjm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zmrjvdhw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uvodtypp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxusesum.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcemgymc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xapmsusv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mcbtolyp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hguoodtk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdzpjqxm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yspvdfhi.html


<!-- 参考信息 -->