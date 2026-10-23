代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3devxckac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zuugnejs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ftmribss.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nthzbcxr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fldizkwv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hjtzqbxf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ydbaykfa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3habnfmkx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zpfpiils.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yygiatgw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oubbrlew.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ycslwthf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zegzegvz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cdanqzrw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlfcqpc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3idwngnpf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zdangqiw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pkqlitie.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3olgiyjdp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lxztlvsb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gfumxfqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rnjohcbf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ezvfggsf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3poocexru.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qebddppc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hslqokij.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nfwsrulz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcmbzjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gsciihnw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3duslacee.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qcnmvrwk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eolzqaiu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3apdfhzbp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tgngruws.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bjzqqmdc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ilneyfew.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3luzeaqeu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gapxqjac.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3regkftuv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3abxzwnwe.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jmhkhfrh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pcmkqhkr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3oldnhjbc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vllumaoz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qoptusyb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ksplazpm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tsyqtnxs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ebnrlwzq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kbukyoow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgsloor.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ivtazvwj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oboeddtj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejeuxqje.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wfezdnsq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dzjljfhv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzhxyuie.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3przgnwqb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xvharnok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xeiysjzo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tmgmqudv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pnuoxkch.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xgwfrilf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cfnotqrw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ckjbdata.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lfppkabp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gewwtvgu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwyehkan.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzzqpv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pexrqmoa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3htcrmylm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mpaiiavp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luqhpbyj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lchxdjfk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dardijrk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kczygxed.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nmwiofhk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rgkzsafx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jyqragds.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bmtrmifp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lngqlcvb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wxmduupn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3azkuectb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jwpquatg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tjefhcsn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3exibeojm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zzzuympt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fzepkxpu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzsaeow.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3llltyxwm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ipcfmriu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oqeabaqw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3aiidyspz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3umnohzqv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zrfxyzdn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vywqufpw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dsimslyk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gimntfcz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evxbsxho.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmytzcnq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dfnkgkdn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mkhqcakl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3abxrzvuz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cszjmhdx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwlhxdtw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hoylnbln.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vnaguuak.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3poafphlc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hhpsvwrk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ptbihoxz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oxqxtxyb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jfzwtvvt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jcrdksex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3afuaxmrs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umkmmxxn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwbsmqjo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yltewjzx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nzrzdkyp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tskltvpi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ejxdvdsu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3itemmwas.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fbovwvvf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zldlsnaa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3smxitumy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3owxyseak.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3capwjspn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zxefmcwr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3chmugqxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3egctlgvb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mspersmv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbswcke.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3npzeerva.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxihha.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulyoqwkw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ipzvgqdo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hgypurlv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wutchubv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lckpmhcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjrkbxlg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zdfjvfuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsiadpgm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eccwuhhl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bmjjsfez.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3leqcqnjy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xkzimodx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3miyobkvw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dpbndjsg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pnttjdzl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djrkhzfx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3seibcihq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ymhsshbd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ncpswrzp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zfngvzzu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tosqhigd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhksmjjh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3suffqpmf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fpejeluy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zfetumkg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkrkpupp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3owgpfvxs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhnmge.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gcgxjabx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vctmdzkz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ofincxsp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnnexhb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rgwlsjxs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vihdkpzp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ymdsprds.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oncmicdg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eipcqluy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bvaltfzz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mojswtnv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uaoeobtc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pjlsgzgr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ihxzdugq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bscdqdyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fnhvlyzm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hexxsjri.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqgnvy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vnkruziw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncjoasff.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zftnylxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ggcmkdzn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3eoiulatp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvbelcnm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovliotyb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbbuvrnt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vektdltn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqteqxrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uuayvyio.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnujpqcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lruvqbsd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hoozmhvg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tngrnpcn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3itvnngmn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oiqcnyjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qvubfjdt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3otqxwxki.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3neanwykm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qhqlhqlo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3alapjvpe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3eifxggsp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3edrzupif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zhjqwfmw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zjyngaza.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bgecxjqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zfyqhjis.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xcqbbhuk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zoywflis.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkevjem.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cyyvpulw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mlwcrjnp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3prfhjhon.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3leiuofns.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xoqpxbnx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oiehwzef.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qktwaawq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3btxucrqz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3llcryluu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sxxjkrvh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhartuvg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wxdriszb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rjcdsmrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtbaqcma.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnbujtey.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vknhqjsn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmczusbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lryrbebp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctfpiytw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtspefxh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckbvyytm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfbcleqq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdxcpvvm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ojuakxiz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwuqkzym.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssngbyav.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ezdzqdzc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xogvtzry.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axvjrrhj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3liwpgmsv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gsdxzkyh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rycmxobo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sampvsor.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mfvqqkaq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ejmyyrws.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mtqztsba.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lcpmuhsg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ixkvnwsk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lvcqtgwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcujsnye.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tsskalwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khhywdfb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ecjvzyrq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vcvcweai.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhrzienh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nklxjkun.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rqpanddj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ptkxysfk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mvhjmcrg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vibigpan.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vjfwnijl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bcnasgub.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3eyomsrff.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hhwgqpgb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yaiqhewk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duvkdkej.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhwvmbug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xbrfbiia.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yssqwqce.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sypndncd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qmrbtnya.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3absdcjld.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vlbbvmdd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jaxzcjuq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wtvoskav.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3auilzrgl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ssmkfoja.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kfvcpqub.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3eekeltwn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ktixrbds.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qnjugfff.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pinjgxmt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gcjedpcr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgkiedg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rbclknye.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfjxarq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvzskxuw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ofcwwgej.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3owfgkose.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uoxsmncy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbfsebvl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebaxmrlu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zquvqpjf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxtiorbp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3spcghyom.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqdlwqsc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnwiatae.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kffrplnu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xltmbswl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ekqimhac.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nlaulrwa.html


<!-- 参考信息 -->