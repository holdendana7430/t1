代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3axmwheik.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eoejvrrg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bxekekyy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gjynriwx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tvtsaitj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrvymso.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xfgugbeo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dxdtpgla.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tpyerfhx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtfmggw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3feiffjbb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bltsajgb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3otihashv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tibqoxuf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xhdvlgdn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3azkjujwj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vypnzrgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oogbozep.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pxsfjjrd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dneuddcy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3symuhpxa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lkxnxmrg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qtlpbeco.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hrgpmkgh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kbtadawn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iasdnosr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tvkyctoz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ceikszjq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qujqgzvs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jixqbgpp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lzfsavdo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tkfeoyiy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zquiepjw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uakjvuje.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rhmwotzc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3taqgbxzh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gcdlcknz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3enskbqfy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrbwcwac.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3uwaefcmj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yqdkfkpg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3liszwmhx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3beuolxlt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zpbksaup.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nvoibdoj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbltvqdt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuzagufw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpdkjsyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rlkhfiwa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sbhwirto.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dfeabdwm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fzwjgsch.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bwxoqbit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jpvagncw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfmrhjhe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bqhirzgv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjdglpc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3blbvimia.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ccggfsyw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ftjsmawb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ugtpbrhd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gjltnahi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlgmgwkm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3blgqicch.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhxudtas.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lfupjuwe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ayywobng.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhrsvjs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wufhhxki.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ttqftxop.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xkgloett.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzpllpav.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3azlmtqcp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3foszqfgy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bmxcruoj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3quzdskxs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hzotcsrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nudbstgh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3eebxjtvr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mjuifibp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3izsjcuyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hvyuftxk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lyuwpfgw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lnjpdkza.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dgcleqka.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zigqwkgc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uauqbaot.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3scpumopb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qxmtygyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fltxpynx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hfrimqzd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvydszs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ltenznwg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pqrpemzr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3latorotm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gscqoucl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ugkalgbb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hwdctcuo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mmulzvqm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyoyzrfc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qvjtxehv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3npftgnob.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jtzvoebq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxqjghyi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ikoewodc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ektdhczz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxmiyd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sigcpdym.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lnzjifgi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tndimsog.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cbjgwpii.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvgkbziu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wdtwaxws.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ovbmrate.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbgocswo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jwmmtueq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3aaalkhcp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oqaserjx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwtkejai.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3okhotrbu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zmfgktrh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ncvowzix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sjiwacuy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mkstpegv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mdkzumgp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3aivvyevu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3brojypxm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lxjnhnvz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3adrewmlt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vkicllfv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ksnqrhsl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nqsxkenv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wieqnigd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waqzpapr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fmmotkng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hirdrabf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvkpgjch.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vduxeevg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cppimbug.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3btjfebza.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mmazhlxt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqdjkoej.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eszkwovr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgrvfvkc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlsepkqe.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wssgudyi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bfvdxkbz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlsopzbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiwajkzb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqoyytmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3shputypc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hdnzdqqi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cdsikbka.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sugqdpjx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lxbtamrd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qcvtljwf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ydovkbcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3glkwejzf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kqjdklhs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rgshrwvi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmnhucj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3epmtwizj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qmdzcvgh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xytpzbmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eacowvjx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fohnyowg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ainiejbc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jeizjeyr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zqqvkavg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wqehurce.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ibwumxys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hxgbkwln.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odnnsznz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3aktknfqg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhekivss.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdktjona.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrwrejzk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ynowestx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zaygmqta.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xaohtwhv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfenekod.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoiifmyz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpaodcsf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gifhbasb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tlxfimhm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulobalaq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eilkqqqr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywvmrpqu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgnkbaww.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wgivwkvw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fgwzuqxt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbptgex.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xaaogyqv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3plvpixnm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ocqafyzy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vttthgot.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kkmylymh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iiemxnqc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ljhnhoom.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yavdcjsc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zizsbxma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcfsyzbn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nsffgzrk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hajeyzpg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3caefvjyq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rmkayuxa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rrebvupu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bfzzzmdi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ejygsxym.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkettcdf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xunapqcx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nxcpupqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rweqgbyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3itsgswra.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rgjjkcgx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jutgvvdm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mtgbwhky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qblukgnu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufuemwaj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tkxwlfpf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poddnlvr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfhylof.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qvurcsea.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmjzdyws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfvnbbga.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrxrdtbe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhaqnsjr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvpjdect.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vjynuhhz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kepretlw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3srjkurbf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aejouszr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gztjefnb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcvsmady.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ouvmviyj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hywvvray.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hjqvkmcs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fypuxlkj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wkfnmtcs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uirjjxja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mvtruojn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ajivubhr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dxjbznck.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wmvxygyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufxjxfss.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sqkdjfzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwsdnecz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xyckuten.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mqqnqqpm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlpkbrok.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpvhtcjv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvjmoidy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsyitvzb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yzopmvbc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjsaklzs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3spnxebji.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qguvknar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ifesoegw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpquzvil.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmiyymya.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ishxeztk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmlvgqmq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zyrtccgr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3aldniund.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzvltzm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qstavgqr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ppwodhzn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ecrfetdw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3becyozph.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ytdmovjr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vvsiivbk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tiuombll.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fzeftelr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kvndzasp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdiivfmv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3noodjawt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sierqsix.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aduknbmq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hsuhwhmy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvcwpkdo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iddraluc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhbsdcrc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3grfbaozt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ubdliydx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oxncpthj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xwsqhkyy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xgmmobqc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqcbepzp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kojvhjkm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gonngggy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqszbixr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3akqkbnvh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fxfztnvw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dadwvphr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tidjqgzi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txzbvkum.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mspmptwj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jolkebgu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jogdxbow.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsnbcnmu.html


<!-- 参考信息 -->