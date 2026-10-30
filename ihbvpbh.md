代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gucpedagk.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpbkyhrcq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/guykhgnhp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gerefiybl.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/grpbiapcp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtpwyepxh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/genlmttoh.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtvearety.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gjxvypxzo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/giadrqikh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqnfgogke.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gjldkflxo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsslyvrgh.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gdmzgfwbl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gksankque.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gigmiyoll.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gkfnqkadz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gekoulymx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqidyuowg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glkqwrstr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtjhxrkhu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gjcifxiud.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gizrgkcqp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gosrhuuxy.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwyzipyzq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxfusio.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gqvbkrfya.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/galokulsg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gouwmexer.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghivcgwfs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gvzofklse.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gpxaxrvyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gnjffcqai.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gkwqktupd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gejbbgmtk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/govgqasbt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gljzztxxz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gflsoothr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gyrgmvqae.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gaoeytsio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gjvtketmg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gvbqgvlsc.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/godshjrmy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gtixssljn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/grfqrofwt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gknmzyrkz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/goiyeajna.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gdohrvlhv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gpxwbijgq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/goaolhbsc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gqoxowruk.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gmafzkeew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gxuxeuaia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gpyhxdsdm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gxcodbwgn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/glefyvkac.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gvtcdjvkd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gnrcraggy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/guzdhwmaa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/guzbirqus.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gvjfvyazi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gzzxfcovo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gfzghbprb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfqkyckvj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjidyfmyk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyniowxyg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gufqpvjzk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gvuvcpbco.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/goykipwwb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gtdepdycd.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gkdnnbnhb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/ggrpyswrf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gmyewhbvg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsncetovd.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gcluglnzs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gwlxcqmof.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gkikmfxzk.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gaqlurlwd.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gwkhnzckt.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gygslqpni.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/giiuyyqpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvihzeihe.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gfzonptye.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gqtjumpvo.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gyjncnaia.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gfuxkhiwd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gutjygynl.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gwdgovawy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gqlmyrjew.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbwuiwxnf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gczdhnlfw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gthhdlqdz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gchcmdwav.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gpjnlguoo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwlfqeext.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzoevuuvb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfzughvkr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gwhdxyevv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbldrchut.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsjijaugk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/guwxxdycy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gajaiitjf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gdugiyjpp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/guitlytcb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gmuttyelr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkygilizr.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gdnuhmprq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grlqgtshk.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gaoemrych.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gukfgqytk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gurdlwdre.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gbbjmchzl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gzsvmhzhi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/giioilhwa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gbpoygkdv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpgntwuyq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/geldcrgxr.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gbuhqkqge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/guffcueiq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gofmhmgkl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkmjmnlkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gjwxymnfk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ghhhrevyd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gsnhdpwzk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdofkfwmt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gzvgofjsa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gghobhyqz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ggcuaifqn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gsbjepdbm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gkpsuiaqc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gqkgkwzuy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gejpsdtjg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gwlbwgmhn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gxklflvkd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gygcgyzen.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gqugydoaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gvloeekhw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gsoampcpt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdoxiwpqs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/ggvurqivc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gyzibleij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gafscsikm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gybopnqyf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gcvkadehu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwugbbwab.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/ghxhdjkrj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gazxoposn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghcwuqdth.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpwkrrkyf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gelgroaio.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gohhjeijf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnhqdxyjs.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdqchtwwm.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/glydfdndd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfmcvyexl.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gawybifwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyflqpvxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmihqprrs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzbqyjoeu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcojsdkyd.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnrlpehwf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxsipdkmg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gjaxggmlf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gcnlxtkol.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/goiibbmrs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gxmziwjgh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/ggktncrlp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/geyxjmtju.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gkjkemubc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gtjizlrwi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gdsvpeokb.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gkzfwpvbx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/ghwrfoodr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gdpmmyuux.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gyyoozago.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gurvkkuxc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gbcpkhgjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gibtatlbs.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsfdbzmyr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grpvebpll.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gfekzfchi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbxhemzxf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwzrodrkh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gnpydoivz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gzcgyvbyh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gtwrwryfq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gzjhrymzw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggibznleh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gqfitofji.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gfrqdcmtv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gabezicih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gfmuzysgn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grwsouahf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdsphafsw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/ggpwqekld.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsqcwwlzr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcfbcfcgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkifqbusk.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gippdokch.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtaotxfvj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gklpjakpu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxltzvwkm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwqbxshat.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbqvfmnop.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/ghcgmzhem.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giuygewjz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gbrbghtrd.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gskcedpkf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gbadduqpp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gkrflizpb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/goqzjdjsi.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gyvkosglo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gijaencrk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/guctynnxx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gnkwaqajw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gppmwgege.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpkypdfze.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gwvdputzy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsiizllkg.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzbestobd.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gnuupumkl.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gbrsvcjet.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gljkbxczn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gpwitiqiy.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gjpijffwj.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gjpjjwepg.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/grvyxsygm.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/glgxmxpmh.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdjrmiess.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/glhpoulqz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/geuofggqx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/grmcztanm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gzomnhfwd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqbleveqi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gurqdqtzv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gbjyujhnh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gyskdwwqv.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gowjnoryw.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gcgolongt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdjzmsgqk.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/goaymvpev.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gtqcwenby.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/grdfdchei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gkkzfiykw.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gphshrnrs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzansgkjc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gppcwqvid.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/ghegaaexk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/guaicvwne.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggpazjger.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwynruvjq.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjnbxbbat.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdlkmsjku.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gdlrylxes.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/grjibzqqc.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gqmrbhjbi.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gejynquqj.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gvihgoirp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtpijscqh.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdwysutqy.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gegkuwzgg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gknkfhhjl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/glzkrhiut.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gyjwjksea.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfxosnirn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gdlmjepll.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwguzwmhb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfywpobhk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsejibush.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghtgnqhbo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gcjxboetr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/glnxqmzpf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/genwxslbl.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/guxptbqvw.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gvpksnvxf.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/ghtcparrp.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzkyerzcn.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzzxwlali.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqmxelybw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/ggegiqayl.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/glpjzmrov.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gwhonxgyy.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gcweokagr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gnekejmcf.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/ghnnnunuu.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/ggmpbzhly.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gevecnjmp.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gdtdwpgnm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/grovgahkb.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gqfweinkc.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gcktadgqr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grtxxxekq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gjtymekzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxqunqei.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gdxqbxbkm.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/goymihoke.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpdbkwtdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gnrypvmpd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmflyggox.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gjyrogebw.sHtML


<!-- 参考信息 -->