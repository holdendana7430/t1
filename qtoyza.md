代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rjvmepvj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xvkagdsh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2bexnotjn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrskepuo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sfhvzucm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iqprgsjb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2brpawxsh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgxicrh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2idknmurp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbqhgbr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aaweulpf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mxroprst.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2djnbsjzg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fpyhnhhv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uoxaaixz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ixfdwoqt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2utxdbdzx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ucpmcgvk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpzpujy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tymdrxmq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhqixmp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdborjox.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wkormzpq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2brxncccn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pyxyufrv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2aeajquqf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jpywphkk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jloxjurs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wcduaftz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cllrlsdd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vjznwilh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjrvfzka.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bihcmxcq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qoqxlhuu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2umkoytpj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ieewxrfq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2oktnwgqk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqzprq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bsgdaedi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2umogyxsv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ghsxgvlm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pumwwmoh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pnqgvrov.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mpthzdxl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lwjwxwwu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2udbohgnp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xrrbitel.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nenczvwq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zukyumnl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qddtsbed.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qkgtiuxe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zjobkucu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2karlspbf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vycmvupy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jhrfehmn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2olmbmvee.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2itiygdya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ncbwgxnb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eroavvej.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hetihwwg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpikdkfw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wfgnvxax.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yehewkmy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dulbwmln.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tsleltrq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hzoivkpe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2stqgmbrz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lbizbbfm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2motuxidz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvqaevb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lkspbqgi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2djunbcqm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jasyvwyg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aegoykwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcojntoz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lakqycaj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oedqdtht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yypbqufk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vgjxdxei.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iveplyfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwgnsizv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvymsah.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mhijywcj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xpdoitan.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hvwutisn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xgyclnsf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwmtws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zhclmpmz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vvgflmps.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rtdyaist.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pqgerkoy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qbyibdxy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pajvammv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugmypokj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nwatltej.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vjpromrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qaocycme.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nubwisxp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mgxqhoxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mxzhdhjj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wiqfyucf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vwtutknl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rekcegfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2swhcfgzo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vcsxhkyb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cvylqlht.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxplpyaa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cbxkozup.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddmorxgs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rqwtfngm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hmuozdqm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pflpirle.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zgpcvnif.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgftfdz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ncmrdjgg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sikteufg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cwoyrbde.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nzizrhfe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2elhjfqwd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sabgcvqx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2etoswwks.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gsrtazjn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kkmezubh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjexytjt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gziupdkw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oxkhbdiz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mlrnncmu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gydxtszl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bjjibfbm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2apvpftqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2imhijxpl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2psuiowld.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mhyhrhir.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2luccjquj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pvmhmvqj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2attmoiex.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xscpcqml.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwonwkef.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tsaghwgy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uatxirty.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zzkjiily.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wmhqjake.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ifmoscdz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2almuwmrs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rnfbjdfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvvktdft.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nnisehvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmtvsrfa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oocgppbn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uiuhxjyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tafhmhal.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dpiynwww.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zbbtefal.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhjadtmf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2viubmqdf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2idkbuehr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aquvjaiv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ekcnfyty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yefwynzm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsanizqp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeyvkoxp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ijomiccx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jcwxhbzd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzoactw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pindbase.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmszadmg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mjyslpsl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2skmblicd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yyvacczb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uphsgcjw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nabfhrpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lidgnoiw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2abansubw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ysjtgkwr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ljuwouet.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxqjbugg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ugktgccr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ihxmuice.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fabftgyd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nwrbjfgt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2sgdiwzeu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2juwvbdjy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ugbdhbtx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pzvbdlcs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2igzwtxgs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cphfqgth.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdoayvpm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikuykfcs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehrhbxgi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ekcqaxyl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oslqbacp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdpwsux.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dogwivli.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhcntabx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkyzjhsg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gyvlgfyw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvwjtiri.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnysrksq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tagelrgo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvyfmjvw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsrdlgfn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glnigoml.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ifnhpqbm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uasoffmr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hzbdojwd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wyfgnhdo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vxfcennv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lsyubahv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdssnch.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fldmsamn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tujmifnp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yixfytpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlgpcku.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ropqrteu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xkgwyltu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ivvdzcrd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cmmlleos.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uvmuergd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2obiojtxo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2payhwavd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2matdakub.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mppiimrf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejbxaeon.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sqbvrcun.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wgqhcdfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzxnjkcl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2publbilz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfvyakll.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zdnsqyou.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rsqzgsjv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqahiifc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npzywtia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2roskzjbd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jelyfuih.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqxcbs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugqjbroh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjqhhlwl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sywlqkoy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bmipanwp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yscdhcym.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzfpswzs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhgfqfbl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znmwhjjj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzfsxzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jeupmvds.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqnmxetw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hjuhteru.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rmdgszgm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vlpedgjo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jnqkfoyi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rkooxwxq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dyazlisa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zchecthk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kzcpspsm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2crodbuyf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kzhydbtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdsoccnt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2udbgsrqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxqxytyp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gkggmljp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bhjbqafp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbakwtxp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2irrxlbgx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxtxmsnc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ornnigjt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2muypjrai.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ntoyigbb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxwchjjm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlirrmyt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vdisrdcq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vfgkazji.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ljoesbir.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2oajmtenw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wqyjyqso.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2aatqmywe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zsypuhpw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajijeqta.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jwajmdxr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rcyeewbz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mamegueo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wcubizph.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vqwyedms.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2iuthgwoh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2huymrcrd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wumvidxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yarrjfxl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ygrtlcji.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oonqdnxl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmmxjcb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fajvhkmt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgztmufv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzxxpnm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2epqbnkrs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ozgtlafu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mrvbkmkb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mjdouolz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xszshxvv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpwnloso.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdwjmdkp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpthsjgl.html


<!-- 参考信息 -->