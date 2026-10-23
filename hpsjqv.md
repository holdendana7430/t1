代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yduodcua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ovoytqrh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3maevidmj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qmmetqay.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dlhlzmol.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nkkthwhn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yaaupcym.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yzuzzanv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhzsxaxo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qatyxvhg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zwgtircg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vfzrpzwc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bekubolb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3attrgnbm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ekyglplq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vtopexom.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3esnengha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3obbykanh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3drqwtbes.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ewooimxe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3iyaskghj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yftcfuxx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3icrexqlo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qzqvliyj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lkzcsfwq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmzrbqr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cwijxsmd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlrfxur.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cfnilchg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulsumfoc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kyrhyiqq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxoputug.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewpsnpex.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jxanvvdi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3todpfdmr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lzumqqrm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rhingtoq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wgejbqev.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3otnxdhta.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3heswxclw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rckgxnfp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgmpncfi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gltoppwv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3twrxvxdm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cvwimtgx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jupopstk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kxxtkfpx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vfnpyufs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gvdpqbig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mipfppsw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zwzlxeyo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jlslsztq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3exqemiza.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blptchpe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3msydcewl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3meuuggqg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hcgvtpdc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xeogwvqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3upkxyxyk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uguyarar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjdjejvn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nygftzsl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hhzfuwum.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oofglujn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nilwtzsy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bpbdilpa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcczzzi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nggpybma.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzpevtdv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wedqvymy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jpqtlali.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pnaiiqoc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjelekej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3muouqrnz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zqafaimb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tfdonxvv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ofexzhcf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kkmdofhe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mnuzhant.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ushftmvt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jtuofhkn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3woswcoes.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gvnioetd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pelwcbbd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ningfzyo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tjftawab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvwwoac.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3incisjlf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ipbhzxzg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vppgoqbv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3friiaazm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zrzcexgs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dtxkmhhg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3obokkpqn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lfnxxhwi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tyjhralt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rdyuzrsb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vsoritvd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sqtznbsf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxhzhdnr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dxcrolsx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tycfmfrl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sxplmupx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uhwcbwln.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjvxlol.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dttnthqg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kdkdvxgh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ponuwrmj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3owzprewc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3erorompq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dartkcfy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3skwgdqdj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nunstctq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvdgnv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xxttwent.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tvyoeyfb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pxhwimuo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lnolravr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzzfottc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yfxmohxx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nlrqytgx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pbhjcmnc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3evgboelu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3moahgfzm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ledjmbdy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3oydhoqih.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yodkdcxd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fufjvark.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gkjbchpy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3phwdhaal.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wywzsnch.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3acgychgm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eocdppcm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3audqdyjo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3notrzwrk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wlysxwhu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wlxokraa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xiqgzbst.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uviaymlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shearcxe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjrwdcmz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jrhnirtf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hmjrkdda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jgsdeaaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zpgwgieu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nmajsyiv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3faukeand.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imhjizxf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akjekken.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwoxhggk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zemkthls.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xulxfnuo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqwgmxtf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pipgusta.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3psukzplr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xknmotmj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ugoqeezx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kabcdpxu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wareuwnh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yuqnrkgz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rrnrfvwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dggjbrbx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mafftwdx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xzlelasm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3omqtmsde.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vpazpftn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jcbyeiqz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3okbxwqlp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvyvaozn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hyzjdeen.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3azeaqstz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fxhlbyso.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3upvpofua.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gwffuxli.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pklzbyoy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jcnyadyz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jhsxwwvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3praxklmv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqiwbvcv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svsjcfvm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcqeebug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oaxmfnpp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ruvlfbtz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itagukdm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxflxzmk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3csxyzsdt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehaymgsy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zpmsdcss.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpanfotl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhsahvtv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3opxwbfqm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qemvmftc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djmgqrgk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3omklfgif.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dxqqpjkv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ytuvsbff.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lcfhxdff.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qhwencko.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wtmyztcf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqspgjpb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qgxguitz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hkyivpkw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3obvkkqvd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rnmizgjp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfwddtb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gpkdtnko.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcrkbrc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mflpfadq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bozpcdxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pxbdtiil.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vtzwywps.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aisjmoxo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uvykfbdj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krrwapsr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tdiiwxxf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yskiukuy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dkfevrki.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3chimxfxt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ckteufbu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ksrsdgwz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3buifxukq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3beufbhsp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yojwybln.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhsamvzk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppwaqmjc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoyxubbl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dnfdwxkl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccusestf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcidyuf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3woadahfs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ehyhmpgn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbbbcwny.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yeywaevl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smjqixnt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrapfbie.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3izevccne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3flryuvcg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvidoume.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rvsffmtu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3metdwfsp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jyxjnbww.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hwkmhebn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ujavevcw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fjyiojsc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3opzdbyzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rgaucvkk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tzyumwks.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3untkclnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eafwwhnc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rbcekzga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3envdnoqu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pgzxrocm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vkqdvixn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3esbqfozi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sgjydtqf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxrjssr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3olqmvjui.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ldqatknh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fmvaskaa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gitkskqa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqkjuapr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xgspjpma.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kkyfakur.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hybrplmq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3sqrtbtyu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bzggbvxt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dqvfnsth.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oaclsfid.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ysqlslhw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jushrupo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bcqrxzqo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dkzjiyuz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oqppjrxx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xrbohedx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3diavtfro.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gpzsxfgg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3unmjylhg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vmvexdym.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dfbqnoar.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cxkhdtll.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozguyvwt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhfqloly.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjzehcxs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3beggawid.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oqnpyatv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzcqezst.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tfvbwptz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tfkrqcpq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ezahkmit.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3haqqctsg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3otzrvmsa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3phangqap.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhlwdnjc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jbflkrdf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jsurdwss.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3slxlzzpn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lejqfdzv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bslettoq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bghmtxjv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjxtponk.html


<!-- 参考信息 -->