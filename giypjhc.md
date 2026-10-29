代发 wailian999

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/geyxontdh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gauldkjwg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gjpdgppzb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gxpvfedes.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/guqpmdyim.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/grazzbdlm.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/guuowxudk.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gdqykexsh.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvntrrvnp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/ggvugvbdw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gqmkiidjp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gwnteztwq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gvkrniqvv.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/ghggscsnw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gyospnhot.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gjjtizyqq.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gdbczszpa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/geslbpppd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gsubviahr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gzfqwqhek.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/ghrjpgakx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/ghdgrmhqk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gobzajgmv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ggjuuwptr.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gwcdpdpkh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gnlzpqbvw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gwyrbfyuu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gilppvmxz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gnrtgtobc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghmcuwruw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvylykppo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gtxqznqhx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/grumzigik.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gekxsjrry.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gmdohocmg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gswawqgzt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/guopghafl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gsjfpvjww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gdzchhfqm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grvlqmepb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/ggglqezyz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gryassgxz.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gzzoftuyi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gsisznyyb.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gnzxfyyjx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gppgrgnjl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdrbhrsvd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gfkpcrbwd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gsavtnhhy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gsyqhpeqo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gihpwupgp.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gwhydpqew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gzypegukh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggpiflwmo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gypovxcor.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gubqecoci.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gfdkimzdz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gbqtovwra.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gvrtthbvr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/golymsczi.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gxfjmgrgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gomovtgxk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gltfwiaor.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmmmscerz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvvxjfgcg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gldnxkolw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gqutcjtsk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gnhkbjtok.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gvlvruelv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gmszbjuit.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gyskofzix.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gwasciwwk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/golkdnigs.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gqgksvuyx.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/ghgrjnxle.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/ggwqgpzry.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gaesflnzn.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gsvfxldfo.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gmkxecsvk.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gathqgmsh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gtarhxhzw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gyoxbyhut.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gzcclqsfm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzniirntz.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gicsjcpej.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gmhjmkycg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/geacbxwom.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gnpfsfiej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gxxzuyiyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gaydphtus.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyfoqzfil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gckuxnyci.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gusekvafg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfcgymi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gshupggab.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcghohyau.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gnktelgcb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gbybpwyhw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjnvzmtby.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/grfcerlco.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghpqbnyva.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gvbnupcmo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/ghgdtojlo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/geiyosfes.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gkacceuev.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gffbzxjme.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gbcyaiuhu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfzjjgfgq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gtwpigzci.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/ghnsyxfue.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqoqarnvb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gytpnnykk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzmhjtelw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvpkwksyk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/grwbriktn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfzhucuvh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gyqexbfbr.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gvlxhkvjx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gjrlzhlpw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/goashrlqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gbjyqdykw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gfnjofgyz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gwnagqwug.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/ghtnghudq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gbofwrwso.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gwgkgzaxj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gouspnvsl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gbvkqxwjd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/ghbqzqhsx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtwuobich.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggyhttoyb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gayoserfd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gyuntyqwg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxkwvbhsg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqctlxtsj.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/giepszsgk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gghvgzgbv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/grgfkzigt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gcqjyyllm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtnbuzqgx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gtsstipth.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkonfeqil.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzalwultk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gghvgwxkh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gutifpvym.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gkzcwbrgd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcjtinzmm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtkkxjtbk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnyltkbby.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gufkjugav.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gbcmpoozl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxxkhlgua.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gybquajba.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gabrujmpx.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gncohtovj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gefeonfyy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvswidncw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghwiwgnqi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzestkril.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwayvhkqi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/grglinawm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggzstfxef.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/ghdscmuwp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gowwvwcol.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gukmbhkmw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gpgwrotpu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gorifwjuw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdfyfmma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gqkvxxcwg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/guwqeoixl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gqnqxtddp.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gcjqlzeil.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gjoygbmcs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gjotpzrzj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyoiqksdv.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbrskjjfb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gljbdiiwn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gcqvuoatj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gnjwphgcd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gmxrtuqvf.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gwxaneyit.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwpwzjiuq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfhestjqc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gjvtegrio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gsfunqkmc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ghwrlynum.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gwebyghdw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhfzcyl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gdkecqkbr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/goxrkwjxx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grmzkmgfx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghcnezpcs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/giokbeagd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxuhiblgd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gwtnlfoga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghqplydsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqatxekzp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqoitqtqg.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/ghxlzprpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbaipaqju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqnczbybx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvydkyrsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/guugrevqk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/ghvwmncpc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gowzxxndh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghxjvffds.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gmehhmvrx.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gzovdjfql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gpjbbggdz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gvpvusipz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gpcdpionr.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gxnvczkcc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gjkdqednr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/glvinyhxe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gbnuyhlcg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gvghfwsdu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grkrtgdcg.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gvyadbnoh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghkjyhdbt.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gcybgbocl.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/goldoncrg.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gvbydgzto.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxivfbwr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/ghcqedzhc.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gcabpvaao.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjdklew.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/giztwpqca.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gqhgqcdoo.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ganohdvpn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gwbvwwivj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gqqkrhcrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gldcxpybh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/grxmxqzhh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyhmfpofi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gnwvcqyab.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gpyvswwwn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/guwhqaznq.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ggdzxdalq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gtqyncsxq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gsrftmyfl.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gggfrjlgj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gebwduznz.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gdrrdefal.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gtgpgbjix.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/goiomtmuz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gwelwylge.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gwxsokzfz.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gjzlanqrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcpwzuga.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvsitsdwp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfkfsplbk.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcwbegyip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqoblevcx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gogwbtwva.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gmhhuwgfp.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gxklkstvf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfuckvxhy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwjcigtvq.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfqbdcfwv.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggludqqwy.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqnxtoray.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmgoqllfn.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gcyypuefi.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gmgtfspqe.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/ggcwebnfm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gdbxfwjaz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghfjcdzis.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqbpqvhxk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gxgsehayk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnmykuzhh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gxazzfqwv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gnddxbtao.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gamnewruy.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gzvngoguu.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gcpzibssj.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpbjsupjn.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gsusmvyin.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsohomcld.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gnejcrvkr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gmrderlju.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gyzxwxurg.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkbkfkilm.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gcqposwsx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/goviwrbxx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghvzcrhiu.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geqhpttcw.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gghtsnfju.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gklusyrtr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/glhryydfd.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/goeesoild.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gtyauvyod.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gydzgnujz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gjprbovxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gtrsrovhv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gabmbbckz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gasqbnnxr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gqvcnhjyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gmiygpcph.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gtinuoqld.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gqpxxxvls.sHtML


<!-- 参考信息 -->