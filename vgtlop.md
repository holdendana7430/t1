代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oiyiszpx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zllrbpjg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3veoyotht.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbrazdq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pfpniumh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uoaycine.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wcvazqqx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bejexaow.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrhmcsp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mnsvlpbp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hwugplpn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3imgbmqkl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mwzebyah.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uhthgewv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aojrtiga.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ovyavbdf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xflvumjv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iozuvffs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xhhhytds.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kpauoghl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uyajogvh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzprdrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yrafothe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xsqcxuhw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kphvcseu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kfxmbslo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3idoozteb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3phcjelbt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvqkkjev.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qxwpiumb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wrpgxyho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uakfkywa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zrcukaph.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tzoyffjw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hcazzsdi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xlrryvll.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bbvwddju.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vefsvhwe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwpwjbsx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hzfysymk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hzsbfbdd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ngjczlry.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wvlbfooo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ukizzela.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wficzjwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3taufvinz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jsezuctg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ggwpnuje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xygsdpfw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iktcsbrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ihatycrx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrhluotr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3aojkmuqp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hbcixosg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dqibvhrz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mzetioam.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bndzactd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pnpwiufd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xzqlnkhk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jqsbvgpl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zibpjyih.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bitgcvpv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kkbpjggw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3upspmvcm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kivadtrs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uiwerpeu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yczhrbrk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfofgpxp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wnwmcuhl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jcfgkcsd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uvplkcub.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rcyyxyqf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qaokkugi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3emtqjhzu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ixnfkiag.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mkqbltgk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hapbsvpn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xrooaeid.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjxyfbjw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3upgtdmhw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yepalmfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wpbnluqk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dbtntjzk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3npsuiarq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nvwgvflc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jbinilpf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rfhejxkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rmlwdpgr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pzuqfkzh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vhembjpk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jjhapxbf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3itxxoswp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3penfejkl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ylejuazv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpylqp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wizegvzp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kgmjquql.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rsvdxdpt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3oynaulvb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3flrssmha.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yskwzoot.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eklaqlct.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zoatufjd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vhhtuddc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3eutyissx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zbibndjo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wgbjzilz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lzkrairr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nnltozjg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dzrpvjzc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qkbjchaj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qkwogcfj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lnjviwiq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3itynvizq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blmtgrck.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yxmztuur.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3enylokfz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3stvbwrdd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mwsnndtj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kveztxey.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xoflbdpl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bvrfxble.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlfpezzh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pnwahgvj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nungwelp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oejswyue.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gzfpmovs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zmjucwkc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cgvrzccq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ftdrgpqf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tbocgecm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pgcwyspd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ubdmimlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcipjktf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3iwqopigh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmzrpf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oegoqqse.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3eyhefgpe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqjykbqp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fcoypdwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nvoxpphb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvqekkkd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qrhgqjwi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkixnro.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3acdcdowu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kduppbqe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cizjwszm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lrzlppfy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvsqctal.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tukwaaut.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cqanjbah.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3eyqkznpw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mzaelfpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmncjwkm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3clkzrzlq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mxmmhubc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3oafblvny.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3febewzso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wrhusrwb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yikkzixx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3giklenvm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ruzynnna.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3udzdiudx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ybcqglqz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dscuqezh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gnvyomns.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hajzrbzs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3buiosijq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxhesbh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kmeeejbr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hmvkyznd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gqqoinnm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fmxpugkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wswkaqkf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujqjvnjp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltcetkwm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbdkxger.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfobseex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wnttnxju.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vugsnuyf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fknethut.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vlpjztje.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gerzcbgr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xqqjglkw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkcknkag.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfzfyycp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3opqlhjaq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzerdlhp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3liyfhjsb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3huvqfzzi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vpvhqylx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sbvnxtqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3evvcuvfq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vtjrfaax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3srdqbdum.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zwogedhe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xqryovjy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mhddilza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3akwhrgmq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ojjfvnre.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3afsxunwl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zszuwsim.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yxtmfxob.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3srtklxnw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmouklq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjfavnqn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wuhxuqhs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzsceute.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3utcxldcu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqbhdfyi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hayaybxo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dtgmxosj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lmlbpsep.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3otbhopqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wvjhkdka.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quoepoto.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xuyimoer.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yvvxfrts.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axkgkrfx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aiekdvtj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqpsbyks.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvxsqnqk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oapsrcgd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izvtdpul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjtedjyo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjisksrz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pdhfirrw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwlcqsyv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whcenlcy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mexgopob.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snyvqvko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yxhtxabr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lsbmsvsm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyfpkkjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nmzunrrw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3phodqvfx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uxibhwbi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cktxsuep.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3voghtvgg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cwzwhznu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xkjluqsx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kwkwpodh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hfuaqgiq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ryasiptg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvwclmkz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3orpeiris.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djyfdcmg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xejneuwz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ywtozuez.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iwymbjgs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cnxswlag.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sojaaqxl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uikoekkd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3toyriicj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ygvhfwts.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmunrdry.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3owjpysgl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xpnhomyn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3clcidzpl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zrzpwatg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mvavafzs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcsuqzbt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pdepzlin.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nyplzgfu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gbljelsr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cjsnzxoq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xrqbftad.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wmrqvmzv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jfuykmex.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3widbtxwi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cqaxyifv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vpnebebi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bvgjoxtk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nbqyszzr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xilkltao.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aqghklol.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unwonndp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rycgycmw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gunfjmmu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbfxilpv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3marytpfc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vefsuzro.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kdumjltz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xkrfgxlg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cfhuldyr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oltooxep.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkmdncgt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vtobhtjm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ccrhvhff.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3idjanang.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uagugras.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wognlolw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3iomryjmr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3teuehrro.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3utyufyxf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lqssifiw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvwgrtir.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbbdsyg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ectvbpwl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3teszcdql.html


<!-- 参考信息 -->