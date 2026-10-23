代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kgdnuedr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zchoutlg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fnsggzvp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fymkbrpx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3icrudmfj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dqcjgddx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3faadmxec.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fmlrlyfg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wbskcfdc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hvyfpmsg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ckhrkott.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3emcvhvoy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ahrlslbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vjghappp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ozutgygg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ugtskiqj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3guxwhqbb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oezyhfdx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hlaoilgp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cdjydvmv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3baxaymmv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfvxkl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ohyybpqv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dvydhjxb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ppktvagl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fqghargv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mvztbakh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3oojyatii.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tqyhzewi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzkrsnkd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xoawtkcp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tpvqjidb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nqyntyss.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dtahrumd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jrztnzlh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vpiknxzd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3imuojdai.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3crmnfpbw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lcvrtcjp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yctyfaue.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hqqoeejy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eipynuxq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btkcrklj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nvtgxfbj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3iptwmkdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqtotxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tzveiatj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3blanwtwd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3abmxrhsa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3btowmjkw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3srgzemwq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwibtmyt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wppoljkk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3atlcbhdk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwkfgfms.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zgjgflzv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gnzmjdhy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gtbtkidw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3secvkwdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vdrqruuc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhlohcr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3raxobdea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gobsiazx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3muwdiztl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vmwpssgy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzlpppbp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yamhvpum.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3irnpenuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3auuyqlmg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wlixdaaq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3edfonhbb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yaowkssa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eiktqdsa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lpcvolnu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hfxsidyn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eidhgzwk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wwspcsun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ujwwiiuz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kzjojlso.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jwukosmb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mwccojxz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nnijtgul.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzfxokd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqmoej.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fnumjtud.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3elqnnjhz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xjmsrnnm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zcuclvbt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dhelomws.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xsmfahge.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfjeojo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cumuggbt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vahlbhob.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wkvqbldt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jpynbnec.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hkamodpf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lfudrgqg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jkwllecl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vfldutpg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrbfgfki.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwbwhod.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvrprhx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bfrmnagr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ptojhbwu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xpbnbfkb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qydwdjnp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vhrdqqrl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3auihnice.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zhszbdms.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cxvnddkf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3oxhhxhnp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cxuqptzg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jdhseopx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tnptzcge.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqhqhscc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3veiajefl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3guhnbtdg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cnevtjyi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3leddvgts.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wlvpaacx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nzanyqmy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ctkudrnd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zbxxklju.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lmxhmzif.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jfpyxkyq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tnreqbig.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bmjlgvix.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dyvchlll.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3klprptmu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mtqdnwdz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pwxzjcyy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xwnjlwzf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3amxooodq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxmbvyiy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dswnbevu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilmlztte.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mydmdzfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uuesrvuk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqxhklzk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sasrwfns.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmxsxyc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfdestav.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fcjdgizx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tysaplzg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpvaalnx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3htwbtcoq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yagczllz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kkkqyexh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xymzfxpr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahljbwtt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ymclmymm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3neqyklvh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zexqpbnd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3urynqjrw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qxxtkhju.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gsjtnupy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nphmvzqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3icsynepw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvmjqyx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dgycvjsa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxgekzg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gprvrbaw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jhkjsbrr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ckszuijb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kittcxha.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3febfigwe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rqsadrrn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ejbqueih.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfutlwo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uhffpwbc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mtqvqckv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3juhynaxs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jekvxiil.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3elcdjuuv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nroiancu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdkzfvk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtmrywvk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rmaybiro.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3awkakndz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdczvrac.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnoofhsr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvmjexgm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgbiakdg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bdrcctml.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghudbwfe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzzjscgm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ixxnnxee.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvpdqpmd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oewplrbh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwedhfxu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tpnfpzqc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vclhpqyh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zzoxwolc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gczdydaa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hoxbjuap.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwloiwgm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lynvgjdf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3urunsczu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rzhrkjnd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yqmkytpe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tghgbvri.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3futmudxz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qefxqdeh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yiggouey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3shyzdutg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzybak.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ikggkxkp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hvhtfkra.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zlyfkoxb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vntozglp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eawrhaiv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3itwbcqup.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ijsmubws.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3onhahpzv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jkkyjnzz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nraasamr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jcxvtasy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3emriydeu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkfkvqri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzfhnmer.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irjkqunq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuivohwn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iyumgdko.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mecygfee.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkxpdmhg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iirsmcsz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhhedpgx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqmflqmo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sewwkhmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxmnnor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebnhzxep.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pnsxcfds.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pumqmysr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnnvgwin.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sigzagpu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rqeswfno.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3izigbohq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3febgdrly.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cxqgfrfn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ikyaqvve.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3azklcsyv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pektpovn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uudebogt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xoikfgus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfhwsaqg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cfwxovti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmqhiswm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xggubepc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mxijsboz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ryuniwqs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfgtnfwj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3osjsyclx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qizhjkyq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3szgrggcg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3utelyakg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yenpqjle.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kerwgsia.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3spyyvqga.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3oklshror.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adptcwgx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kjlozmmt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zulkncyx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gjcwimtc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnmsowdf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zagexrrk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3awonrzty.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3quxrclxt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqdaeb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvwbcbwq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3apxuhomd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yybipdjb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ifhbldhi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gzjwpghk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qzzutnja.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxdhpu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nfqxhyto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bavxbimc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3taunszex.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eyxyfuma.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bafhakrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kyylbdlo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jopdwqhc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hiyqkuyz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tmsvbexw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rcixoaqn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geozazmp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wxxgkana.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xtykuibv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kklgdeew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vitjjpfa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bclyvktu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojecpjcx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hxeuqntv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fcwgfwvu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jevnaqko.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uvrywylw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zeywrvly.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ywzjhfte.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ieydfxhd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ulesgjer.html


<!-- 参考信息 -->