代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hojxmqfz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eynuglku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kctgccaz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3akpkmwkg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oyctbjje.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mndeuxku.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nodeyybt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3goodxuwt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fivwofnz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ocsyfley.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3arvpxmex.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jgrjknas.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzcdgdz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vszdztcz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yirtpjuy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vmqjmspd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jgrsjyum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jyxfnclk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rvafuenf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3idracsvq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zccmjcfn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dcsfdbho.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3niwhxskq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gfxrdwla.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rvgjjffg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xwdvycrx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nfhgaxgl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3elibikqp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vybtpczk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eedzqczn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tnorsbqf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bluntets.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrdxguvo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kaiycgyy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vwigquvf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3heukkymw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3schvupfd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rgljqyli.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qdpgtzna.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jidpavyr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skhmugzq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3blifmgto.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3koqvrjyl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3seugmqmc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vwbvlvra.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gubfyzxx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qiprgiwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3luaywunu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tlgcbudv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3weewmdfs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhmhzf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kdfglfev.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uqyjzqcc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kqpihyzq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zchjcmmc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kitrcvrk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmzspzi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gjvztesh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zwyetwdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uwkywkae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3enwkyirc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vggljaan.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ysfcdzsk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ykexprfp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tlxdvujo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3idpiwgyq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sirruzem.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpaxevx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jkkivyqc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3urgkgdbo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3syhavsdd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wbhkthsg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ljyphtez.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kpxgjftd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3savdxtrw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3beupitpe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxcssea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhhpgug.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ljlvpefn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wzmsfjgi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hsnumoyy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jrskqwwq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eptkachn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iiftfpcq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3disckcpt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pudgnlbq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pywwyera.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jfpmoibz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xchyppdy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jmvzvoxg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kdeedpxs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wkwrocok.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rxxjkjpo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fxgzcjfv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzxhysjo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yfyvyzyz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyfrydzx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dmlwtyhw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udxfajgy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3opkwcwhk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3raasxiut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plxqdadj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jherhnjk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xmcxlgmf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wugwypgf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbkolw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ayxrcvum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kyeevxxp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3idlfiezq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzaaqneh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kkxyfqrh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vwtczwms.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ikixijkq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tvrsowzs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3idetqkec.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mcqdavzm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yzlkdpgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqewjjat.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bnaxxfas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kinpjrpm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sfklaaro.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3acpubkkd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqqjvztu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sqvgeuvu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lzxdmdky.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hjbtefbf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gekxlmxk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nswudsxi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zgsszczu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcmtnqkx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cpewpphm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3reperyev.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znjjpppg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pviyhung.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tvbijqbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfqmkhnh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3duzodwlv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lxejirvq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bwwajdhc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3idvnlmyk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oabqyfmq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ruxbozzs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xtsowlfj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3egntdkdl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpytvbt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iloybhyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lzqbrtao.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrkrwupd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ijuvzmwa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ngitawzf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lhyprabb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3egmyqcki.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kuhtjqfc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3scewojtq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3daeqrhyu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qenltumn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nsnwxppo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xmbwedvw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bpuafgfb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivshwthb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmqnzscw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gbscbgeu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3klfcvgcc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mryuelaj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elcqnxuq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxbwehep.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfviepzs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3veyrgowd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okldzake.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drregnre.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iflzotsn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mgtjohxa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysnscyiu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bihqgosh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3slbyokdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3txghqszz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3khdeeemu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kdvqvgae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tdmiywam.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xbeyvqrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qxkkasns.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ekmyembw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xwygaefg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kshnygmw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzgmrcfh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kottxsju.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ctbwzyns.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrddxzoc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aizzhhqg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xanfhswf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hwlahowc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jelanqyg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hondsfna.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yklwkkwe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xksuiuvd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3geolbhnl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dtoaeqaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uermljnb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uefqqsny.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbnidrrw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mlbvmdfc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vqxdkhej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csykwjcb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqnmefzs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elfshnrr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqejuq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mnvhnrfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgnqpspp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgwtpxwl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdnxfntb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3semmhlfm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3naxnajxq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdfcvuug.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpvuvgrb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsjbhszl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrpdbla.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oxgpmaqc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwjunzd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhvjim.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xmjxgsbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3doqqmkal.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gusdkkze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3udlwslgo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aqkqqzvr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cdzgzvly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dqshjlya.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jopmuutd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3htpgidqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hobliclb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kenlapqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blchupyo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nlbrekfx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tatvmbgx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crabcpie.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlzuzvoe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhediih.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ittmrybz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fsthpqtm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ygabbice.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bcuwvdet.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpssunvm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rtbwgqvj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akhucnxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbhgoflp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ptwxehtq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3donjrybt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vswnsslr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmmkcmrr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eowybyou.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jllawpqy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dewrwbeg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ragqfxon.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jamgmayx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3elwjtjmp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3opwgkgnz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3akeketqe.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rngolyay.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xzbbktqx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3agzuanqu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lcobpzwb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yyllmcjg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ftpxsmdb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3taliafcx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqmvrofd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qigyvwls.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3emrimuaz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3waahwmfu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3eqdkyjpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ztqbfjht.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jkxnokjw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtjhcqsz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omztohwl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kefeocgy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fcyhiyga.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrbtuvtt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hmcrtgeq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mnieuglx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zcgiwaxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabtblko.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ltgfgdpb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ierhqbjj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhgoyszc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gnhkxgyj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bolagibs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kzkypngz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qyavromg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ulbojuse.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmydlzss.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kywejtmd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3grkumhdc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pdfxhoru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xixsvcvu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pymvhyuh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ngeoyqfr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tdfmtudo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fluwprdy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vutivsuw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yhjmjrxu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3niskeblu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gdvqjsmm.html


<!-- 参考信息 -->