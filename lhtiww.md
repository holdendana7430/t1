代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klrqvqgl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hgkzazzk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3senqhije.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbfhvns.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bribwtrl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vcozjzjx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bobwgarw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3npqranrk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjmbzllk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwapaxpb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tpxxgsxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3npbxficz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wxxkbcbw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xgikdlsa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dsodckkf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rwwdiwjm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zweocvop.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxzjtwer.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdmbyyyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dfnndnoq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lnwqfltp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sqjurfsk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ptfdhorq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wqhppfna.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mtbebtvh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpaqbme.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lokmjfxw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qryqkzuz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlrddmk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pkdregak.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3aaaloisa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrbtiufm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ylxoxidj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ywxhhosm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hhxenbee.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3levwjzqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxjlblm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pycwfhds.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bnvtypof.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nvsunxru.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nutceyot.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qzqromwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qznzgbof.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jfebzzoy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gienxsxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3exbtiufd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zjxczdgl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wgufrorj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppgslurp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gmjkstqd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mcjbkqjb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qywjubxa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3skdnaonr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jmsdkntg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3csdpbxli.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxkpcdt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3sleeknwg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3svifihph.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bnacyttx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3iggpdkrh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rmkpgxvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzwognxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3veoifwbp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ajwrzngd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wdmoybbl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dqpmosfq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hcvszofk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pcmxgatn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nwdhdnbf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ewyfkzwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vckqthgi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czjbhgpw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqepjvig.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tugprxgo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbazqem.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkzymuil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qbhpfnfz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qdlazbkk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3owpxqqbx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylneodra.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3opjkzvbj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3brprtusy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qxgctarh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxabqfgu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3evtjeljo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3niabbkzz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3elkegmzx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zuqwngem.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gscttzqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzltjeei.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wgareoky.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtuvgumq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3covrrard.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3aycaizkq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hshaynot.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ovrdipss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3scgyzmwh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kglzqlvx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pzsyivgh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ygmpsvae.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jvhljgkv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iawutgdh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dicbuzzp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3umdfbywb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3juonduzy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3apvfkiot.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnfnqajt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxdbgfrq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3espwisto.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mibvutxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bczaguos.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qqddihzi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xituttgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gokqcgyj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ntppmeit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jepgdgdv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rftovjpz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mhrepwzn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehijiqbm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3syhedvbx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rqtxjzkm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lblkeqxt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vcimykya.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrsbmdpm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxzpovxh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrnyhptu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3odwolxxm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3unffmmpz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3egjyeyaw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmujjcpz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zxubzbvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jstciglw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sfvpadib.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gawsikvq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sjqdxylh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yenofwfp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fnjezjhc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gyttokov.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ielgawht.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kqiadebm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tbqsaavm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vcoptrgk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cigrbrwc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzpwpnke.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwpgjcr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xlluimwk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fahjxxnx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3atzdzyip.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ewakdbuz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gmzhfjvh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vlhmkkdg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3skmmvyah.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bkauzkre.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nmqkfpjh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahqynjkq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuorjjwk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afwlsihd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3igxhmwod.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ibetyxql.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swbuencu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plqupdjt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bvbqkvhh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqpudrxl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qamfqtzx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llzzbkkc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fccdzvov.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jfhdjqch.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nincgzoa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbruzmad.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3izfuswfh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3nsxkjdpj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xnhqumcf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3evcgdhqx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oqwohqlj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fidhggtv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3boqjtbbs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3llohrrhq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zhwkkjly.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wpcxrxpe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rfpfxbyb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jkiyxkka.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejkqrwwp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nridwhhp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3esqrnarj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eczktkfz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbvnwgau.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sjapgzwi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3smeeocek.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hrwlrboi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jijlpylc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ceqplepp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wvlmvgej.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nziuwkzj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwbzypwf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3muvbmler.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlcflkcb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aynttzzt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jqeytvko.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gabmwqnm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dusklkfg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygwgiwqa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ueraxywj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rhbpfhxj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxipbvlp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gprokqky.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgdbymod.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtlxbrwj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zocwoxbw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mozbdxdz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddwglfaz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fglwlqgk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pulcebqr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rrenqcfk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awaspnfj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3arbwambk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lodhyakk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kfibryws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ddawvvov.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zvrrjqhc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mbvwqkfz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sdiyfvkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mhtdzgel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3moulvdmw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tatvknnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfguwffd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wfjljkdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgvsuxva.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rzyboodi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3etftnzgx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3buydfnpm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3giivkyhp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3paduigeu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkoaepqy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zhcwbjpi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3chtrzhfu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wdfqzcyv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rodgtlhh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gytedhxh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wymmlnfm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kavqwbsh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzdtrnqh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bqfouzoz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bljbkrhk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3amdgvcwd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sehebpfz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vojyckwv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3exeqmmpd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ykqlzbey.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gmmmlxpd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ckyrfcbg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zsqnfatl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3symebile.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cosguxjw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ojqbnbez.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fooennum.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xqjsucgs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwnwpgc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3futjfxra.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqjbrst.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfpsgkga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rsokjgkf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttmzkmwe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iprqhnws.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dflmfstg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3koexihoj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmmqjzhb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uyoqsior.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3urqpjbsk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3keirubjj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ztnxaoqz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wlomvqhp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnkuotmq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kuqcfkmy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3whgvofbx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmnjgqev.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wwbuvsug.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vmmqdcqg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zibzujuj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jdhexyys.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3stfmexst.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hruqjgrp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3orwhqkoc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nheczdqt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wzfwtbwp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vcqgnfrt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cfnaqlfg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ssfunhib.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qhagdtdg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ywfgqqfp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rnfyaxyu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3atgxgkdt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ofnbawii.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rmoufqfz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gervlgak.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qphwxhwh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmcvugwh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lzbbnlti.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpofbcax.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3muwxvksu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fpvsetcg.html


<!-- 参考信息 -->