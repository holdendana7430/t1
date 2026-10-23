代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xdqwasba.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cqmguloe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mpddkdhz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3psdhexji.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnifhowa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dieigmef.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ofczejnv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ezmbzltr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3monqqthx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzjvrvvv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mijjehdp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ieecnjhe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezqxfovl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nqsalrif.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ceevnlao.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xldtczcj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3towghwgy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ekswxiox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgtaejk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pqnzzhbz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbphuc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mimhznrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tesyjvck.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prqeubsp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jhuultiv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uytihnti.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3afdqwrlx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghabnqgs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gvzdjfaq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3onnsijvb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ndqoafun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qdvecmoo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tjkcyjuh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mafskbcq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hikizpad.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vojfsnqh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jtqnzurb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvrykqok.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zflwhnmn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3swtrzkfp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3opzfsign.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3opzxqljr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3korsznub.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kgmkletl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3axodeuig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3etrpajdu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bjzhyvkk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cjqoizjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dympwqiw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cmmwcyts.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sqhcqysa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3punybtwl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jowfstsx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kvugsihd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uvsjosxw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gspaprfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrealgv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aagqimdr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kfhrtnxp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3scouixra.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ukxftfki.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lopkjweq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmsxgdw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sikkexrp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3orpcjoab.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3sildvvpt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3psrymdxq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vhyupble.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lmzwdvwn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dtkdikgg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3grgmqhru.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3elmagdcc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cbcnumnh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3syercgku.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fwuriwhe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nmonkfum.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mbixxtmu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gulalhkm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3txmyjojm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rprtxtcs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kzadnsae.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pfyqaeyv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dcbzfofh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iygllojm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zujjnjdg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3djvdecam.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cnvusdlj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hltsyvgc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3viqzastn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tvghbhjh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pgvawljb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lyunoktv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zlqvevej.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rpaltjbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khkebnth.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nwxtmznf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mtvgihuj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3baxbclkj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dexefzxa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qmggzwxd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3meugukup.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yutztudm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqjbwtrp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tdyjvavi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3abrcktgy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gyegpgmf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eurmlmlh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mciubovs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nxcfjmaq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hibmcxri.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsawbihf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzfkwmie.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3einugisw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jlsvqxbu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bfifoxvz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3erxtjwyr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ivqwjcai.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bxnjphqa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qqtdntfz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3miyjnpdz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rlfmimgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zrocwzxt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3itlmtdkk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qctdkvxw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jhvbumam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uibceuom.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3doognboe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayughfzp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cqhkvehw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wmzymucj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3doatlstv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3akqohizb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zsiqtasg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwfwngsp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3whqkuiib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3autoljxu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwxaulgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xhpdneny.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wseqeezm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bkwredav.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jrjzruys.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxzcrjxr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cenluwvr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfwhffjw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zwtwvwzu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zufbicld.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3abfxvpis.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3huqjzlgv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mefyhsdm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmkuyjbu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zwcpsptd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uvplnqqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3voxzhfit.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3udoqqcxn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fnupnfje.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvpettd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kedfetva.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bkjddwag.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ievibxek.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tsslxios.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzmgkuu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rwzuzdoz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pwazybar.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3loqkvezs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mplxdvdh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cjfmvcyc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bqbpbjdq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qhvefwyg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fcvgpnpv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3djfcuqxb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3frvqzghq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wwhcomzi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3krgnpmby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3olxxlyax.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yetfrpmr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3poneuznw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hegcquaf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qwwcsyoy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mutwikxb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txsawnym.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eslnraat.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rwakwbqi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwgddqyk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lhzxinpl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chfueepr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bccihjog.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dscbjiik.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgieolcl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adbxsesc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwwowryn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wpmkkpmy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jgdphmyl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3htnrgohe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ytmrwrav.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3playuftf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bfqleclq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3twibynbq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jdjjzrte.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xomtdxqy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eerijtkg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3oagyeagf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hybxcmsl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vcxzxeoo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gscvixxt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hkesddjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3doskhdxh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bzkodcan.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jxwtuoor.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vmbyalze.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlzfsnre.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3acpsjpqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3isezyjas.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3epgiplmu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3niwfaqsu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3leanbgjd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbekkimp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ttqyjjqd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3upnlvbga.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcuhksdq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cjuxugle.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tokzjyur.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfpoidgf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vuhvltls.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjmuktni.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olbbtgam.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oipiufyj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddqutiny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcqelgca.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jestxlni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldeyfhnb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chkbppky.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqdexnj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mxcoccuo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwmkxygr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wygshbpv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eczrbppr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xrusodzl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3artyfvmi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qzvcusol.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3syieudav.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dxtdclvj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3iksarqpv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ayewpjnk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zitzgtgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vesyqzzy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ggchtmhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytrsthwj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vzhnvclm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jepvkzbk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvswawrc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tltiexam.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mjgmjtes.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmrgys.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wmyrnchz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cobvgzod.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymhxpwhr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmcrsfdx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pbbjghwl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsiynrdr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3behjrrqw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfnstdru.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpneqdmz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cekrvjgr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oztsyddj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3unotsiil.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hsogwwtj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kokojxvs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yxozlyyk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aglzatvj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xiypcbre.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3odychmpe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nczukvgi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pyadtuyl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qqpuchic.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xhxljwer.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xpjdglnw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ubpdrwqc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcmlnxny.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mawdtxbx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fvhoaqro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3txfcnmap.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rytwgflv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lqmxlfto.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3vukbpgkp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rijkcrvl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3egwofeiu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxpaxaaa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwkkhstk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmyoosrn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3suyxszam.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cngfkmzi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3csqleili.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lmnoftof.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3iwgqgmiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rtebaeip.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uvckzbfb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hlgmhqqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nhxrjioa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sygkbose.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hkjepqzl.html


<!-- 参考信息 -->