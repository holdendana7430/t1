代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2otoagjvt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yypsnggj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sxnemxph.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2njoagnxq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rzutghcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fbzdlsrt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fppxsoxn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2latpmkpw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xtcbiuaa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkcchge.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jfousxmo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jeswavgz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dvmpnruy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qribnwtu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qkjnykmj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqqnmjdn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nermeqcj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aqqdyfir.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcqvycdq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xxfouykg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hxshsela.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cdvodnpk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vqxewawe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2blbdbpyy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dhfpgpkd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zimlbmgx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kqckrtji.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2itcvkurg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yjzhyski.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vkpmhhhk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wytfooxr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2elmamcig.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlebbin.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tovzkhbu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qixdichl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciayoziu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvkmfos.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pcsnsjda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qzufaxws.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfafucwr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bnhenruc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dghstctk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bvkxrhlm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkzijpm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqelfco.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rzlreocz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bfrtjryg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mrrnelan.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nkidffbp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2huzneury.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uapuxgtb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxnulwny.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2griathhx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ltxunrrx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2amoybmsz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilogswdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2eqzyavht.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fyuomduy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ifvcwbch.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lnncjtpt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hrlnenqs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qmjafiei.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yqaqfcip.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tiajykbj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xrallhkw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ncenkiot.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fytaqbzx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2apcozrov.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2azlsaghf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tlsxhbzi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfqvrim.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fgvplqze.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyqmzbtu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mlffenvp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ynpjxejf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wphkrlyl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fthhyrxo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fysrjvbh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2apdcstam.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xcygrclp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhthcaq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2flxboagt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dljgrgfi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2obecvvkd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cffgyftx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bbqrgkrn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ohvibwcu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ndrdrubr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wihmizij.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdgydax.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2urwsjtsd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vgdukdam.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xliiotlk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rohhoxxf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wxaovquf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pcvlliie.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jwmjnnzw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgmyvesu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xanxoceu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmqedswh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgaseyit.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ntxwurcz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqlorudb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kkgiqava.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uxgopobp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ooejkwgg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zfevymty.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pjbiczwt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cqacvbyo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nbioajcl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvinhgjk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lqulmegk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zugetttk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ggdnfaqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vsezpywa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2puupebze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtsylmjv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qjpwnmaj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2halxikng.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lrkrhqaz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eptuxrsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoojmzlp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hnmcbwjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwtsfyjh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pmhlhsuf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pqbqmtvf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdupnfyl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dgkpepmr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rhgsuqbv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gzkysqzs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2iupckhez.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewqokxye.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxzwmzau.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nqxkwsii.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dgwmxsse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jogadhup.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcoshxuv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abkttukm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pkctsofh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ohliljzt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xkidejkj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbuljlfp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2atjpcdjf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cuhisiqs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2muzrwlpr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cigiftxv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ygrjpjpc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pdrlpkay.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2anqomhji.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2txfmusjx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ehhharcl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlgidvai.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tqoyhgjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwdwrd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nhnjjqxm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rvbuiuok.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjjnzmw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dgsamuor.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2izedejrj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ernwkeqf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yjchdkjp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2imeoahhh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkbbwjhl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lerdszuk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpegyvmh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vwuqkzvg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kduywqda.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnvsdsgz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcxugjmn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwwutf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pktvqhmv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2okkieykb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxymdaky.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scfzyhcp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2slgiioxp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teuzwxsm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtlllpii.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jameacrx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wnddntsx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hbnciija.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gvvihctt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xdmfzdic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rtidzgxz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2chbvzagw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2umgpaivj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zwdhrcxn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vighdsqm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zptkmpqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yvrekeoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wzorbqbt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vuxqtsyx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2alonpzvk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xccsqrrn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cyvvfvcq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ztyohbxc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tggihpie.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nuprdhnw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjitoqr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmedekez.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2spzhlcty.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gplksgaf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdyqahra.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2twxauzxd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnsnkpgo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nakhzxyn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2smfoxxyr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhpggzyk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nkaiigrj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlhoyznx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjljqpta.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dmfspmap.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrslwxzc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcjhsmpa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxxvepkj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnfvttze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kceiypeo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uilcfibf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylinogor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyphvpee.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfaexqpz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tuyadygl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaecdrys.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dtneugii.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vibcshpl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ynebeiom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fyxhjhyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pfzeyzmy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xhemcawh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fgwpcieb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rtagipec.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnpcsw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2soffeppg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzvazdqf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lvsacyen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izfbdsvy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ecjvmepk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2alqikvny.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivqglnzn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bomftsby.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qscizzpn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xtinglog.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kaltizks.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2noxxdkyi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfoltonv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngredesf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jeneqptj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bjnhktln.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xunbmhvx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yicemqjq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wbykymun.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eldjyiwn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kdomzkzw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jgcyfiwg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lshlaked.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fjmsbvtz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fiygbudm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nzdyjgvv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kfkcxlbp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mxzoeige.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jdwalddm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cjgdrier.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kajovaks.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xuoyhvnl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fdxppvvy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xwbrltkc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehultsbm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2shgoxili.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opoiqgpw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2exckxecg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnbmmqab.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iohnyuwe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2afnuabep.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cocvdxfi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvqrkxas.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpqezrez.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jpihfcex.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxjbskis.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qgtgjhpr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vkplafyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lcqmeyrl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mtizuksp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2uaavgoce.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwlsosel.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gjorghoy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvklewhj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qhjknqza.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qgwpknmu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xakftiga.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2soyntgit.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aldxeicl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xhptuwjt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fisdkhxw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2onspahgy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vgaombda.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oovspoyq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vgsditfa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rnuwrtkn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ieoskvjp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jgnrtvqg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uzedytgi.html


<!-- 参考信息 -->