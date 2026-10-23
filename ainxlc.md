代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sbhubxhb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pfrowjro.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dpxdyxan.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ydnikssj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gvljysrc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rxtpimbh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lwzcvdhw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3czzzwzmr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrcmzs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vgssgefj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hhbipnck.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3krngjguo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhtausx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kmqhdgtk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sisaucow.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hzqixyiq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yzncghos.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3meeazmho.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ikzjfqxg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wxbfvgzp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fzdikckp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3snzldetf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nbhpooyi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sfxjpext.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pcqsyibk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lpyldggi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ltzqreby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lmtogwbb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lotzwvho.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3leobvshp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3azxhprab.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3teluzomg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3btrqluut.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ucvxdtqa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qzbckmrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ccklpvhs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pctkcpno.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dekrqjes.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lehcgxak.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3grittxli.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jilzmxyx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3srhzuicg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmlywilt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dwucjpsi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mihtokia.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pjznilca.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jppyszxs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3humistym.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmpriqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jedlfnoh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eokvijya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqkjlzj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhjguux.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ibvbrosl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cayggpdi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gprdmwqx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eoqqudjw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rrwnhakq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzrlcqie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lyekmswv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqwyspik.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3deiyfjuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mbayafph.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kwhobnqn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cngdgbel.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ugpilkgd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ysmektcx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ncnldcru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyszeyut.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fnhbvlvf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3myxudugx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ciepljbm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ogtmeubg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hhmzwshy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3combbhmf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpoigqek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uzptkzoa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rdoqzlio.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tgukddrz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3azyplyid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhiokvdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sggaibnk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kawubavm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uywbajpa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pctnffdc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cdretvso.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yabqimhk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfcvvdrp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3leciapwg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xbhpbjnq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eguqqbpu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jfmgaddd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbaayphf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mgjkyqhc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qxoiuqix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cohxcajp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqmvbagc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uuuzyhrr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mcynogih.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqtlqccf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3filkxqhg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qywkffkr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gumadzmh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvdqnbr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3myqawyuz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3erithdpq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uqftgzoy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zrejjhbl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ykiggffw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dzrxexgf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3paaloval.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rmsqjpzr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qxxvkbyz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhnrueho.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3shiqibni.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xytpcypf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xowspbfo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3atvtgkpl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yjhgwzdi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lymzvnwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ukencaux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tkppyicj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vpdcslfp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3altczwyq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtlvnrtt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fxqylcek.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wwestejq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dwvzvkze.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uqvapyum.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itzjyeeh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ftretagb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ehzbfmar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3slwldilq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nhrggfkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3psslxnbp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zscqcbpo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dgwvebws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdjqultr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jrmzhqhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbyiwnzf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvvsaakm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cyxkpjsz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slexzfdr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3svqruuaq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ahtpsegi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mxcyjnpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cruwrfyn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzobtdxb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oihbeohn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvuufcxe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ufhsvuao.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yykxagdn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmykvzhr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gztbdgtl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vahqaqpw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3osgsoiul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ndhgraex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zufqbokf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dehrucxl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3crwvxtsz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3whgcljmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iocqotrw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hnqycmvu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3thkoujal.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nmlgqull.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gktvqwdo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vpkgvyaf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfnsrjct.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dmjvsbxc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3evpmqnfh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ekgukckt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hegdbzvg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cnshhwwg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rravaixp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dudsaneu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nvwjyply.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kdgzzvbx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hjrftveu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nmzdsoba.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oklycbxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhilyvpm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hycryvdb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dbjfejla.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdspfoe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwvzekd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gptyfxsy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abkqoriw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ticirwmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayaeueeq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdfyojm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dxrwyrnu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ultanltz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cckbxmox.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fziamccr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3btjcnjgq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3snxrfohp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yqzuhfwm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kpuwshfr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3shvekler.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vggncvdl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gtjzrypz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zqphtipp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ubzonvyl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rkpbiqbr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqlsqdm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cxkqaeaa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ckmgizzf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pamtwfpb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sepwbcxb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gjwlncbz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3muzhidym.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fcorhcwe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3epkawapv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plmvpsjp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bbrggxqm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lzhfuqwo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3spsecxtx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nekidsia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jubxefur.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwybiibb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qzrvwwyr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mwpqwmko.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hljeznkg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sqykmynd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omznrntq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnehdhmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bvwsdyfj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsvwmiiw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scezoseb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwgutvcz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wjdpwvdb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qilwrxpb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3csfyjlda.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igrbonpm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoaqogpq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jaawlbet.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pquirqin.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3szqrndeq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mvychlsa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ossbuehy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3clzdcgms.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pnmroqfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3durkrfld.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3akdwoggz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jfngjaqu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bnrqkuux.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rkplyiic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bylspbvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfzvztad.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tuconxhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyotdjfe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3onhegaey.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sxbslhoj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3krtsuuty.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhizcy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqujaxin.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nfhhrkqp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3azaciiat.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3klgcrwzb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nzqykbpi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rvzypghh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mvybgtbr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axvvcveh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ypsqthxz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzonihhb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kwhwagxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3swrkqesb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bmwliekd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qavgslcx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vjftcxaa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3umpvfdad.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uzuesrnm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pxuhecrb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bkjvdvdc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pgnpqtfz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ilgtfmes.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ptbzhurc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iwxlaotn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xiswrhqb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3alsvjmri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opbjiahs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bynvpzes.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqemxhnl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qarrskob.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iwyovwwx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3conozllo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3exdodxhd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3oafgdjrp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ovbsazhc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3osxsnynh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkmesdsi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cqictyek.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3azgrdwzb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gntnifst.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmuyejfw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jmohftsk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gzopxahk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pvlhcsje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zmvepmwi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neucqujv.html


<!-- 参考信息 -->