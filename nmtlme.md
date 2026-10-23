代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xbqmidxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rysugsnj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kykhiiye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lcfkjfer.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vzesbkob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bemleuaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rdieohvn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sagvztoa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yokubzuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3bjrxvexy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ohzrdxyh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvvdhms.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drkkqgwq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lgshglot.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hkjzkvwk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3llhzximw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzwsxcs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3amkbcpkh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egazrtvr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dvefrfhs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgxuzex.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jvsoaxlb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3acssgtdn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jypuianc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eigbmnev.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dtoqytht.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3flrzmuef.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3webulawe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vkrdubmj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3omytxjcg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bdnkdtdc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xtxipfja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3onedblsu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uawqvutl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rpdyylty.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3inwqsojf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jlxqldxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjjsvm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyjfuuu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ubgqorrv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hyjicpkl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rbsktlrg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ylobmurk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yavudkap.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rhusreuw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nnslclgm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ovmgkpvx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmwewgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnorcnru.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cuzuabjb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ritahrqf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cieyvctm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mcyjirob.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dioakazg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gotoiaaa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kulnylot.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbbpqzu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oybuutgg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rinsjieu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iggdrwvl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kpxtluae.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3toozdsqr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sxqgxron.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xxksanpk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dvjpzisn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pklswccq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqihqfey.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hynjuwsu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mgpzhpwr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3czmnpcie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uolbbzqj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sautpxdd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cturnhti.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3anwdssmc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fsieeaed.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xotxnrpl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3keommfqo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hgylesjf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3niifhgws.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ggzudqny.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hbsqylfi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqzcuche.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pgjqgmzg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cqqqzgqq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdmvxqco.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zzetgzjh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gzbwbivp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3khvdrfxe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3myvkqrij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxbkampd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hovnqvaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wykxcyic.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fizfsyso.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rovwpfcm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dgvswpll.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3csjkswle.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uutmcneq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ceuosclw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wdqeliqy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufhftgko.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtesngzx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnygpflu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gyzxwokc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kxhyjgqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mtncmvun.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jsgeyktf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ootkukyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wfvhuksq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vegnbvpm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3msknhhhc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dhfxjpui.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3amagkykh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hoxeblgi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rjmiffvo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3heypsvtp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uegimxrb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ygwnjaqp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qtkrtjgr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vjxpmjml.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oqwlqajb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qyvkvueb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3esxmgqvq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3evvhsozd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ojbmxukb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3itjlcwaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfaelqw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsdajwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ipdcnbsi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qzohwquz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3otfuzlle.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3maywaxkk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juexyhsv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqoefypy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3avocuquo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3szsbqwfi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvewcu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cunjhnhk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xvklcnbm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiscjbhu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3keosyvcz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfmgyazc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npemstun.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bkzflume.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrsgpoer.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzzpsw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvodygjq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rlgfbjgi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3inzmrewm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ocnqmijx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3luengbrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pjkqdxtf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bpabffso.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rlamijil.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fuamyctu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3aoiznxmt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mcwrulbm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lffavssn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjtafjtq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zpohmneh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gvdhleyn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3umhitznf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vpkcoory.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gisazkwh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yfhogrcz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3stloshvy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uevywahs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgmmyhip.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hqzuehhb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rruqjwtf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uudhnfxu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3aaiotzxx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgcdfula.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3htvxdliy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vwbmjolw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfeovaww.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ruhotugo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uovsymok.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqqpzrng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jknpawrp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnfstgkh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqkmqumy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jscsvvqb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3axrvytmo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxlshbhj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ofsnzmya.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yylodepk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dehsiaya.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fnyyzijz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ezjgsjfh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tldjqzjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3idrtnutg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rltsstxc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rwwvqpmu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uizmmjut.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pasjfyae.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vxtgtnlb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oqbtibjk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3aoktlzrr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pbyvyqjt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3oapewrbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwuihdtf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vzjcctlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqiabvdr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uxbuntnl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gbfupnid.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ompqfxka.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrpyqhyw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oivfniqt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyfenftb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fsmyhlin.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwspdmkv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppkdcxvq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3npiakxhh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3thxuwsks.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rswnceda.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwtzdk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3oqwwsual.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfhvyfki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rhwolzet.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kqzwnhcz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3thbbzkwx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jhhrxggc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3adwohpkz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mtjvzdvz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3awfltsbj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tuixplqd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xgiysfsn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qgcehjix.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lxqutgbr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ttfhfrxy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gmewycao.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zqgkwhaj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3myaucudi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awtnuqzs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3myisbqrh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvlansak.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbocnhz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rpuvpbei.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3paffjjwd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hdfmcifr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nfqlueuo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnhewfnu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewlnbulq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khgdkfki.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3txzyodor.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mivqsqeb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3shthmydd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zyvnvhrf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ktfhqnwc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zmuxtuzl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rqwxamkn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3coqkpued.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aukxxpao.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqfmrwkp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pwzdmbih.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcgmxtbp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xrwpakqk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vkxmizkf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fsitkdfk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cyrpaxxp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hevsxhbw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qwphkuie.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bioyojag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3eixenkqo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fhkkzrbh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gdnhjnjb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rczsfrom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3emnlywvw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckfaydpf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3sgjvsknc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3usgpodep.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyazrrst.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xdylyvnq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gmtzovov.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3axseakyb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zdgkcpuz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qjshayvp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyggbfns.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3osbxcdyg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bpcfhrsl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsdxpjqd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cdwpqdwz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3neknzstr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqajqxmu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3swcfszxo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ejgfakbf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qosfnank.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uhyzxslk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mqfhcvhk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yeodqske.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3btbelliy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3joqqlett.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fnqmmvrv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vpzweunu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3capekmmq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clddgohp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kczbcmts.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oupgydkt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jprweqkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3awdrdfkb.html


<!-- 参考信息 -->