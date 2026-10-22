代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2clpcqdcq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2imokbomp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vkgmqftq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ghajhaqe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ljzezjbt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gemxasqa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gqylplas.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2inbqyjbd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qgozifwt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtnrtcq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gdnbgueq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cygjxvsn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdegcfhf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsgrleug.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eijeymav.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ructqwph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzjdrw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlrwsyss.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ztsrvfob.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zysprvjw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iqroakft.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hbjjussg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qcsvzolm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zrerquhm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ssjtmybx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2slkceuww.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pegvrcuq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqnrjgp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yfvmdsdl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wagasggx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2unmnezgu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzlfknzw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2avvooagt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjvrmmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ltsrnyjl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kpwyxims.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jfaxwcij.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mxevcyet.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uxahakki.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ytcrkgmi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dkfrzers.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2osbjucjw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nyeozgib.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pnjcpqwg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgvkmxn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tlejegyp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vjvcgbyg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cphdubfc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmhmwiy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kuhiqfzr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqmvjwf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtjuapcb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yphltlie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hiklolek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gukbhuvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzvxkxo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hfapawpe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fhqukqmc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2comcxvyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdugyri.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkorhudj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fagwuogo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2aeixrxps.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2grodtbqd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ahajrtlf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ejoqmsfk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zolrwnwe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkbzzotx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2roehowzp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2enyhrvbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wytfhhkc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wsdpxxnm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jwzmbjrz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2agcugjma.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tmwfyzne.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2llbhsvgp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gyoiylxg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ygmilprk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cpdglnvn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cbifibfl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ekfklkpv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sudgycrr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yuyzxavm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cesmjmmu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mjfezpml.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqrwepcf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yhditgul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sfmyxdke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvebmycl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2urlhqfiz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bdzppnnp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ttfaxksd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2exxyqizs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wznbcfen.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xghpyoxn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iteojyzi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqmcjy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpkxdow.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvqhgnc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2heerhgfb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlnnbfgj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nsbiepzz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vxthquvq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dybbmdld.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gitgbqzl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2efaanagv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ttegnujr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hypsuafp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wsyptdzh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2upezzhog.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nsvwsggc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qibzzylo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2infgvpnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtchdovy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtcgxkle.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvfsbgnn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2efmkgvct.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hurxuvth.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cifpczdy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yeocbuwb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2loqlayqb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kpejdllr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2glmecgoi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ghubrntj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wgqwrpee.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ufrcuubg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vvewipmp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ngboubza.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2iwmtxhvm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhpfccmb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zefioxhc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2djjxdwom.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpzescpz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wensmrid.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ynrtjtze.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ixxjnnof.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2imhfegur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjaitmle.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2iphsmctn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odpgbslf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pktaxnpv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2whwknawg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brauucof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gpzeshvd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yyzlerun.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lvhrwhqm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lapgnoaj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhvuebw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ekwipizm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2abxvownw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pzxcnxjl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ggjsbtty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bxdjpfio.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfpeoqyi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kueunwgm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2krfbwfad.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bdtyeiyz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbgyvuio.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2byijehfp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljswyqpf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uviievcf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uqyvbgud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gsoohnhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jhmpivev.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2czzaqwxq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2afcknenu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jkyvbtwf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzlywdhy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2imedhbsf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vdxuqavm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2raqjlkos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfepbdlr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gbhzhatj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xglkxxmn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vzsnpaqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2znjeinem.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2djqpktjy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nbofikxw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwkgumbm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bblptdfi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmznrkwa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vjvnsyzn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ixfrfvds.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsrlmdbx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eutzlbud.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2tuphtugq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcevccla.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ssphafny.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uciwznga.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slmdrqgt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kuryibki.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypzkmxrd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfpqnpzq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qwkxpsrl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tritterm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tcjvqmth.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kxoubonr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cmjcrlis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xyjqodyj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ohrjlthl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cpkfarbn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vtvbwgnv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xoncctvc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wilwseew.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ziipobqq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ibwiiwxv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ifeoeboj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dllyvguw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrheews.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxueqxg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iwdzivid.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2akoyyuhx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ntsyecmo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpbenzch.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qgblgtqn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iuidwhfq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wosetzgh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rmdhcpgj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2azgflpvl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvejncsy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ysieblhb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wjhazoeb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azbftogc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fknlzbhe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltgllogc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbivxvej.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wlaghayw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfzigent.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylnskmhu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wztdcbsx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2driwmylu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2srxdpihg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2maovexch.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhpfwrtz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdmagdre.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aywsyxbe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lruoueky.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnnqqsfv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jtmrovuc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2isripudj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2olnibuis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zkkjpfow.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ufmgmitk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uwotzmbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tprxijfo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qyfnmtqq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2djsxuenv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yqqibzxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhbrhcph.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2iehhdnqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2marlkbsj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ztycyjsp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yiudqgty.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2amajsnur.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yxijgawd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2miveakbh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sfdruoou.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2haouihly.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nravxxss.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnfhwzpd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2srsghhor.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kxowociw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xomppcyj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjwyxik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpowhrey.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzswwewi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xoqvduxs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsiqlexm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dlpzwdzl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2otqwwcjm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kdcqtahc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2joznvzdz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vxyxwcew.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jaohthwh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xyqfqxaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qkaconxn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zqyygpoq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vkmaeevv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bexzglju.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2msziiaqt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uzyslagb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kspstlze.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dumxkgyv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xupzjdbp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cclqjujm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kmjzitcc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2erguxnhz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hygtmsjf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pwdtzzzw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qvshkijs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkazar.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fcbzkslg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mybdhjxs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fojhggxz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xikphzkm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khzxhcyu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dlfuwmuc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2znaovbps.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ebyjqzxj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ygnscpgn.html


<!-- 参考信息 -->