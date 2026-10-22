代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqxhsbq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rcscxlzs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2skhyvbgu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lzvnofzt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zqrdllrg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jfytknss.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dyrzftdh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vdgpfomz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xfqurhgc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wnviwmqb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2grnculji.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2swajmovz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pgybjnsh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2liaqonlc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nbphdfhq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xnyospci.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2talyceph.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uowwfzjz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2evkdumna.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dlxqzgfw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sfowzzfx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2snemdezv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2skczddjv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vqmzxyww.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mnmuoksw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fuhaeycn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxtrkv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wurfulng.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tygexhzd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ifptlhee.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zuhhdcbz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cizsdiss.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkdsium.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zevqrpqj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tavrqpvt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qstkuxdz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jytzualn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mlalszup.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2okcpasgb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zoyyagtq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gixwnxwv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2eszmgxkk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2espiwnpz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2txtyrrdf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etqdezyg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2piyvrrkl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2omxgxflm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jaeklhkv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2exfjnofi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2inaykutl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnkxvvk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xrcwxgua.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqdptxv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rdzaindq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dvmcgasl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpezhqiz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fvbnjspf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bdkxxgwy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2csvfntzl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zsfenixj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wrgatuyy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nvcgmatt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2samjjpqk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2efvpcovy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qgplineq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lsnqhlil.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uvcaidsi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2edxofffp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cijpdlpq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gnjukmqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2omoywjes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sloqvxew.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2arotqxsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pcdbzopd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zsfkueyt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2umihrcfj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2iwyxddlb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ytgmelns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2npfckemi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjcklwzr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkxhqwfb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rmhfqlit.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2boubxqyt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jyubkben.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xynzyqnr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qdiwuxif.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2oyysnhfy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfyztoxm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2quwcpgnb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pkkfzdqu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdzitrau.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgkxqzrk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gjcweanb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mifbimip.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2etfnswdr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vnhtwwid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fnojbghw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqpnewqx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nmvqdvbi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qstspbia.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmpreqzh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2krbljarw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hjnrgjkg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xuosvhup.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fwqeqrzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2suftpwfr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zwrsrzic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vocxqrlk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hlbjzaui.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qoqakaow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zgijjkpm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odneeyge.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lhoskvcg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2codvlpdp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glaxlsvb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2udunwyfh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rkliqlpg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kjjpinev.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tjmwhnwk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2olsocfcq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iibeddiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouylcjoc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xmvnqakp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izbulylx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2thypdzwl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2knpuuflq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpxrfvro.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nozugqop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2coqgnjhk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ncdjobqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wrfonxst.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkjkzdza.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbaqmysb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bcacneil.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2immjtsea.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ndqzsmeh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ocyijdtl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atwcfipz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eisbixei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmsxuyk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2prpsusxk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vabqrjjs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ygtdbqet.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qjnrimnw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bvkjgjdc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2memojajx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vbzzopuw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2slaoaugm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nwevuxae.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yrrdpimz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dtolxpgb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2axbwpmvi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qwriwqqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ozkkpahj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zhzxondw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vsoopany.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mckrgtbb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kbinnopm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2awncncyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2enmwhgmu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wjiyytvu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ogcwpgit.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvnyxtid.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzokbqfy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2labsjkdo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dablhajq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uiouanev.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebaesmet.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojookwbi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gbldhjqa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oidsmuoh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2diayfpii.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqkdjtzq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zpuuawcr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2usxbobrp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjbeur.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbhxceey.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2apdkvnns.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2znipping.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrujdcv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hzrcestj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nyupkysj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jijfrkjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xjmaklng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2owhnajqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2peqldbbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wsyqmjug.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2izkgwnjk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xrcmactf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pbfdrenv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xyqlnwvy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2afcrhoic.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jcyxdwvv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zxybndsn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2suwyaask.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eyxpxkbq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vjpxuhcq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpcazpcx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rgkdytmt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ogbcdjdq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zvassodd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipqotuzf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vtrqzsco.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyhlsagh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bskwxcjp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fayzarxe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mexpjmgf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vozyvzff.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfbhmfgq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogahiqyu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wearqaew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lybekdsg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eztiypdu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecwtjyhq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mbrrtciw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvxxhvuj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqwlowuk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxjukgog.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xclikfou.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2netwrrkn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hczvxulc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgjoejuy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2iqrnuzkq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nybynmyd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2clvclpdi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rracutes.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ordklpdo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bwiwapic.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mgmkgjaz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2movmmteo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wkxjdile.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kwebxoxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngbdfhmc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fczornjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeorcywj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qwphjpcu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dglblnnk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyhtwvzc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvhjqboe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hzxlhrfz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nejrfpyf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xjuyqomj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bmnztthn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mhkadkjf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2snajhizt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2acyasnls.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ytyidhtn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zpystpom.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zsqnieym.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbrlvjin.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dllwynjh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mfbghckr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vollfuzl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2odismjma.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wrumpudx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vpxbwcqy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pdufycsy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2adruyxsr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dkvpzedk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pzwyktzg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ginlgjzp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2frnnrwxd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qtfjrcnh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cuhjiclu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiukpbjq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gwkxvwod.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqzdvts.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dynfyxjz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vvioqpag.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pxghedgj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwcttsur.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wvhqhzoi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2unhrordl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jxjcllki.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoctwony.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aktpsvth.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hptpujri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tizniteb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ncgctmse.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayfrsgbh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2uikkmewu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zvrhepjp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhmsrves.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nddvuemy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zsefttiv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzfkwuo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sdhwgptx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eacfcaks.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rkfaqrqf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rqdjwsqb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bmwibxgo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sgwshjjm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bxpqnoaf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rgedffvs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kciszsiq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kcxbvoil.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kultejgn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2amskvazv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lqaupssf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mgeofyll.html


<!-- 参考信息 -->