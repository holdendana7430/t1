代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dtkekfie.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3arhapxdq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3swkduagt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nkiwjniu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dinujmav.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgftdnk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ulagyacs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iytetjdw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3migdokny.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnfixfkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wtlpavmr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wakxiqly.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rhsrlifm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3snjnvbum.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rxlnhjui.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbnudzbd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dzrnujta.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fyazygtx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xeayfxan.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3twqvsmkn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bhofmdtt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nchbzuzb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3okoywezs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pferrbpl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jcqzcled.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xutthppl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cyswuwwg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ayllatoe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3btqddhzw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3afaupxmn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3idgtabml.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iodqeocy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3aihbhenr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3trgfbqqr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jprmmjas.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3czrwvjem.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wxieaxlj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lshgpxow.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bkemtbph.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3phxwtteu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pnmzujvg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wltaqjir.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dnlhjjld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rwdklgpv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ufwytuyn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nuxykhoh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3twvjgreh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vdtyjwyk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pvbliyup.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ipotqyxa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccsckyqj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3msizjkpa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xaibrvjq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3egwdpgwp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jcsgtlws.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lawalgne.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uqfiryqg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dcucvssv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vogcjrsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dijczmzi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibgghtku.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3khyhqxqq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mqvbhrvl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmogwbvr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxeaoyj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fxmssaft.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mmhmoolj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohavugfl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ibangquc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnpovkbk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lxxqglcr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hlukivkl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xjfpzrzl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tykrydbf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nkihcgws.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vxsmsurr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3plucesea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sibegayt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfcuvzc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdqyflj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jkxcqvyj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3alhjbvdw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ligjgljd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3azhwocwu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3iiezfijt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dzwvoxgh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qsephayd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3skljlges.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmqopgv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rxusdjkt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvadxpw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rynmhvto.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cmybumir.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uijrvxdb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3iwxitgfy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dggexcob.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3umysquoa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lcywpbei.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bpxrcxdd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvyuniaj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dqazjqmw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fuxssffp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pbmocwrl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jmxxvuue.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rnsubvfw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uamcjvlv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdhsgnil.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqycdobv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cpjrarqv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tcsqbhqe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mjbtwjbe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bwwrypss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3auesjtld.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ixzdehrl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ecjgkihb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3staecnwz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3swhrfwtl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3smqrvcvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbwlcrns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijsccswe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3crtoyktt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3baexlmqb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hxszmjvx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzjjgxwg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjzypocu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lkucfijw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tqwaxavy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mtgrvidx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qymdxbgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbctnhhf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3etptobod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noytadbr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kxpycoml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dthagouf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfzclwus.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rygteeqr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3scqufpnp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjyyajvx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qejfjopl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkuxnvha.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzxfocak.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dlnyxhqu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cimfnxhz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dyqxkqun.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xamyheha.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixpkjpux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kusetixk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxgwtawe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ptgpachq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3udybonhk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3egdyiczq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ghfqisss.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cexihjua.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gbcphkim.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rmmnosxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqnktoz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bemcirby.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hrowjgsj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3igzzgtjg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwzwvdkc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zddaijaj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xvbemcne.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnpheid.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ippcextu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yaxedyrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3caqqzumg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfmjzfgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3glgoioru.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3twlhdhrp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tftzkkty.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbvlsnfv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okhtkjom.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dumypuvt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jbrfkduh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3htkillub.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptozfvpw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohhslvov.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gjefrneo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khapaejv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ngsuynun.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3liyoddzh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iygfqvfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lmnlqekd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stxxqbjz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opnrpqqw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hspvgqkd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wokxpqxb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcslcyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzsixqun.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3swilqwur.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qoajohag.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3htdgxhwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yzbaqjij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pceyrrut.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3imgspxpm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wkljzrfj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bwlfqcxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnfnxwiu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3quctygxt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qlewpcoy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ikfkvgip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vvamwpch.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gaydqknq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxfdwmuw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jqquphwy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkygpbf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzogspyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dfeswulu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zoswvyea.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zzekxwxe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tcmnjrql.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opcbcmlm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fddanars.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yxtbupzm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awvlsoua.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xvoiwyrx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kodkkiye.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awmrrqry.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pinnluqg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivtfhhrd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzpavbzb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwyjltzj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3paxuzxvy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgqedtif.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrmdkeiz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzkpmjuw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxhagotx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ecordjep.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ppddwhhc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsyivusx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kavkyxei.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rsprcmnh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3etcnmipp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3riryvbdv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uwrzaisj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hmyutrhd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kuthegdd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rlhbfxrc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tglsluyi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dqbvxknt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjpyygkk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wpyumrra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kknmgyds.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ltfcnqga.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kqyxhvsx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iitaxfuw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rprchvcl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovewyeus.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqfqsdam.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3muhotspr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfybkust.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tneplydn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjmrmnax.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bochobfp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3besgawds.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3feahlmdm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qohjhpbd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxlouwku.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dkhelcpr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmzrcmft.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3apnxtnic.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3axtifnwc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pnwfwyfe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3opzwbplr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kcykwirq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ttgtrujr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lybdypkm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bmcujovk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jvnbrbqz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3biaishxg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ccotzihr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ctrdyqqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tdpfdyal.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zxlazatt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuuecwjs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dygswdxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vfbiqrsi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gjinetie.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sicpyzmq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pexjvqjh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3imjpwqqc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xbqthemq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnnmsiur.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3josxgawc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qdvbscgv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lhraajsq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cnssgbeg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gufntqzk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gqcpsrsf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3twijmnhf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qwkgwdbh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzgkyyz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3anhdftgk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yswdvtwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cyistmpm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3taezonpm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pfhmxpjz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3aasxprvw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cmlsckmm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3daszjeiz.html


<!-- 参考信息 -->