代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oitbnndj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rimbbobt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bolwrgkj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkmsdaq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2epfukttc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pnkitswb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiribbd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2umqaquqv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfjrxlbc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xenmdxim.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2snxtdwek.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qflvwdyh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pribfjph.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vopcluwv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wcrhlgqu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2brrxhyjk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zuheolxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xyghtqfa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ftpnxcni.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xnayincw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uztzaiig.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jzifbdwk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnuvbga.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrjicdk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ugsfwzku.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wcltnziz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fldlxoxv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qcfbiutv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rwynnlnp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bqjlomqg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrxaqhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jpeliolu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iynbyxqe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ipxgztie.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fumsjvpi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vwzfknkn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kdvlebeh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2brgiutfl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2txpwktfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kufilmtg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zifcvuvy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oneldash.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lguitcqp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fphntkay.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdlbzfo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lcbhkzis.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xysmlclk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jkwibsmy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsbgerp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qqdvteka.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rwqilqnd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmwvjil.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zgntrcmb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qfaoeohb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtyveglv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcjmodw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqeprkn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kevzpzvq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2clumrhvc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vvfhpzcd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wnryqpro.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ifozjqgx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cxjqddsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcibkcto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lbeqmogy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fdwtakcy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rsmbcodi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhjnehb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lozzrlme.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2expkpcme.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nlicjfln.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2olfxhdyq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2phlyqytu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2byjduyvn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ndrlrhvf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ichfkxhe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jhyyasns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qaimaevx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fkfzvdpu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jsnfbfot.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2czkidcgs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ppgajibi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmiloorq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvbhnwy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dazardzu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zjsdkyvh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oyngzsuo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2famxmngs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kyussssl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kaajwgyh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zdrxeqeg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgoygbz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eogzbzqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2awrpjcpb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pfblgegc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tuggesbu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2soovznjc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wcrnkegz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2besmpugx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xcwlaagk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nadtftkt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2klwrsqod.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxjlceqo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iyhpyfis.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hzlnltts.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2myzgmdxo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ozaggrgu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dfoxloae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wfiecrwj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2swrnkngo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxikxkfq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pnpbzvst.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hqrryvhv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2clydyyzq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxabvawa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dcvcuusn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jajcazhe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lacismzf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uikwnddh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aibmtbwg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2udzapedu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tigpeqiu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibnknmpr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2grtwfkup.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kiklxoyb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aixutoiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xxswahlg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2skkvrqqa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vftvlsux.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rrlzrjzp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2awgypcgp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fomkzhaq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2blghyvex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jggtmqqk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dnekessk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2engadvxr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xtybcwli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jvvznupm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nawnhiik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2woprnqnd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtlvcm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mqbryaii.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bfjgrzjd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pipkozej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kkcrybdq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qijavvcq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vtsprmsb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tjkluwov.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvvgsoya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plufmkpl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2twjjekyt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vshvmbtb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lctpvndd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mrogxbhy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2opulryrn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hevhswxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xqitdfqr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zhhavwap.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rmdipfly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ftuqptqh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xjuczpyf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zvjoeyqa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lbrepmxn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzjwlkat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fukyzotr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gbuwwqql.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hwbgvefo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aftcqixj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2clxtebuo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xcmpbgaa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wngufwrk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zvhkilfq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kdcxozzl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yrejuemr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umofhpyu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gitlboqh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrqoofly.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2myozahrb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rmykogsy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eabmqdbq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxuskvoi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zeulwhru.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2troffomt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2notyhgan.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifquohui.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spsothtw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2unydntew.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvcjwlsl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsvmxdsb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyuzinmj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ivohkikh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jrahnnrj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wzglruij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2olcdgxjc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2awnrpabl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhqakhus.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kcxnluhc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rctlgyys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xxcvtymb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vjbaxzrw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zqhksvyc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvinsabm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aepzejed.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kmumwdnj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2itjzggkr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sowpuqkr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vsgwaequ.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mlwlvyfp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dczmdnuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwkmajbt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqdkrjzu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ocjijvkh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2atnviatb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uqdwosiz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ccsvtndh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdikpvdk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2riegzazy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2arqoigjr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hktzzgrt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihkycxne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbctfvwg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atijnqwv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2idkkmfgo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vublzlov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyhsolls.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inxyolmx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lldtrxme.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cprhtlrj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbjnhbyo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtrswifc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fibtauma.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pdecekkp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dvyvwsqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjajhrih.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gbotnzin.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fgvqozmi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jodwdttd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dujbkzhj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wiopkwnv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2edczdter.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zzzzpvlt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wuifkzcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bfcarqch.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mbwemfrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwwoqhpl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2namtvqca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsqepsbs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2akqjaeeu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tqbuyyur.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2biepohuc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kztsmalu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tziccboi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsigwctf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fnoqllaj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ytuytuch.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2syosvirw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyyqavej.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2muesvtdj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lpkldzwg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ooabdlgf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xqvvosaa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhhwbnw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qtojzhmc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2shmfhizv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jlpgjesy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lreagowb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vvwowgky.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2auctuauw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kunrbqsd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tpbajmpd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tabrfqfw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qpcvgwwb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2phdxjieb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hthvfxde.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dskyhohy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oxznmeuc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ofdpnjbf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msocugad.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2naxgdlpb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blnqetqg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wblmycoc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nnbgnmcr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjzlsxpy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kufnuhrc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2akkpxxgb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrelagdb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vizrgywq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fprdoiua.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hawakozr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fpksvteb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2coqozefi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2svcozjrp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wjhfxdkl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qmrcfsgh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hpqoxgby.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilaslqvb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzlycyvm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqdgnou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pkyjftyb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lldariul.html


<!-- 参考信息 -->