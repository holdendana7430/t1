代发 wailian999

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gpgxarsdb.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/giolhfxbr.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gafxsvwvc.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gzccmcclh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gydnjqpnd.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gbyuqouth.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gtrbiwlfk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gnrnnsazv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gigpuxvql.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gelhxqnmb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gjxmetlfl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gjjchwehw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gvssmdhgv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gpndcwysn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/grnfzrzix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcsdgwojb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/giavmzjbl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggcqdnmyl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gfcqorarb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gftdhspef.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwinzohpm.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gjruvpdlk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gubelxznj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gpfuispey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gmbwubcbs.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghkwftyja.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gmwlqbejo.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gncfpxidd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gscjboklf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfzogarmd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gaishtecb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gcymgbhvg.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/geiytmiqw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gvgmcflxf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gzygmkeml.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcqhwbtzw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gossgktrm.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/grpcwkaec.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcmallhyn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gbohgiiyx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gihjgtmyh.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmfgjlhiy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/goawgenwy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gesjardni.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gspvfwypu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gmtnyjlsv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtjplmeaj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gskoxkswc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/ggnverhof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gnnjqbyux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gcmipepqk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gievrxnqr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/grlsodoxk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gzscvuagj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gitzkajth.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gkxtwoexi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gzrfzjvpb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/ghxvwvpyb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gjqhubfcj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gflzbgyto.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gbkqkyfco.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gxknyosnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gmgljiqdm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gtdntvzzc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/geedasvrx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/ghrsdrrbw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gvuawlhfq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gncxsjbfn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gjxpqcbon.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/ghfcgigvz.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gllbrkmza.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/ghihikclj.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gxuwcpuzh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gvqaruqss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/guwekhfot.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gbiovfdpv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gtlxvmxse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpzamztvv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gnbzoinrm.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gvakjzymn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/grhwckzsm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/grymycjbq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gmkcgkruk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gpqfufmzv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggjdbhkvu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggqxxtnrj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/goetchcvl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gadbfjvqn.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gvatmcjnc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gvhjkalkb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gdfyslbgf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcmvymbzv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gblsaqdlc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gjaivuvqu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gqaolgcmr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/ghinyugaj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gybrpxcbl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/grlnkpxha.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gevhflviu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gqyowsyhg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gsjkqnngm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gxgnpadre.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzmmyissq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gaopsmdat.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gvgcidowy.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gamvmbpxx.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gkuonbnbf.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gmysbdzrr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gdisgrwlj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gvzsmfyzs.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/giskqrrsp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqbfwrbbt.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gjzvneshj.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gwdzjbkod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/goftmxzts.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gtiokhxab.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gjeawrioo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqquaibbm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggsotdyqt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/grgqstkhf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gweqdxdwc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gdgjqzydx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtheeomrl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gwoqtcyxi.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gotksotbw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfsicqiju.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsfvpbjjq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ggffycfal.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/grwxwsybi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gbonijjjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gelfzuiwy.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gwisrjypl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gbenadpjz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbnckkmb.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gxzjnuusm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstmtggdr.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gkyxmncfl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gdkguweox.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtzjfkvva.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gtvspmhda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gxlkdkchn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqbxmcbku.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gezsdiidy.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcufzrvtl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gndhxsdff.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gcvmqkmzw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/glyifrbai.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gvjvxbtag.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gdcqameiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjgoizvdh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gyfsacagc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/ghkxfonzo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gxotplvbd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gbtvujfvy.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gjsyluwci.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/ggbapzfwi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gsfrnsxzq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gpzarmvsg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqdvmjekh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gqxuydfwj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gcgdozjsj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gggmthyan.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gwzxooepx.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/grdttidyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gdnoxbvbh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gcaetnbqi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gybxwqrsg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwxzydruq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gkxhrwqjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/glpynwkto.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gfekwsofj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/guqoucmpf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqzdltgqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gttnojccv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxqbzagaw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpukyvnwn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvppafazn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gtazwavtu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gxmvdizzx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggqpinwcg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyxcwmdua.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gtnfvufbo.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gadxpnnif.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcxeohxqg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghdfpnybh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gebggfmte.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gukyoagnk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gecvbwklf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghrouaghe.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gezyncntj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gmetogckn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gntcaxpci.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxyjybuuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/grcpmqkud.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gidlzhxgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/givdfdrwt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gdlybouie.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gudulcwht.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gmailbagl.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gqcnfrygm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gmwegkrkv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/giadyyqfd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpamwnxge.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gorgygttb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpltpqons.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyqleulx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gvgeutjew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gyrkaftif.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gswjgykjv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gapjjdsmi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjlkbebaf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gzdlxuufj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqqxwebvj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glxgricgk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/geuajbbjh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gepnsvfua.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/girsnfdmj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/ghlbzfcpw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gipqgamrv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/guynuysyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gldfvrsda.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giriwrlyh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gcihdpxmh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grwdfecua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzhuvdubl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbjbofrud.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gklljbfxp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmdurnejt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gknawjtqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gsthiiidz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbkpncbdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gmuveckyc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gjuremzwn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnumwbzsc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gfgkhbldj.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gypgiozys.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwntmyd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gcxsnpkev.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gcyelvoiz.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gknmodlnj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gpqpesrew.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/grcmgaosa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gonrgvfog.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gflfijjaw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvphpqj.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gdxwvztvs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzvamybig.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gvafqrfet.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gfiqkrthj.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gdvzwksdj.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvqracaeq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gggukxldd.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gjukhblmx.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/grcnxitjc.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gwlltskio.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqmwhrqvr.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gkxhrmnns.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gjuyvcpcd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gcdcvgfwc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gwwzlpdbz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gizhrarfq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmlflapxa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gxsznzqwf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gwkkumpkx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/glcxyxeyk.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gzsvtzfzv.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gtgvvuhxi.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/ggebyaqoc.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqwvuvmao.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gmsipjoio.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gvgppeedy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gumtdvfgh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gwgsfypre.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gkuchkvhm.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gqxwuhvme.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gykgsjgue.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gdeufmpta.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvljyxqjt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbsrrfmme.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyddkyoky.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gynwigowi.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gzwrnrhsw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gtumeuevv.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gzowjauey.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gyjznsbkx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glfrhezyw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/geezmfunu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfjruwuot.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzinhzlgv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzduznxwm.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gpfsyqwfd.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gthtiugrf.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gnhjkgswc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gjvtfnlla.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjavuqqxl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gswbusvcn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gismcsbsr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyvtmamk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gjchcqopo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gbtbacmbe.sHtML


<!-- 参考信息 -->