代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ycazwawk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bzjxeasr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rmjbuvix.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3otboyfcd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rdhkyamx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kefqldwq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pfcluxtc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zcyecpwl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kqiydhmm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lghzpxpy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pcjvvjxv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xrijwsuz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bzvwkefi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdyzezpn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wouzeano.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3haejlmda.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bvchoxbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xnallkku.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ypobmlwk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3klikspdo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kraymqzc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wntmfgtw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jbntyusk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vsaoancu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xumqrkkm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wvwxaqkd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rfsyzrqr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nogdvkqa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jntsmuqz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kkypzjkr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3usnfjdke.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jqqrrdjb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kboukiqv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gatyagtx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qzndafkr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jishcury.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3odcarvwp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mrvskbau.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3czzoajss.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eeoimjto.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyshgse.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3soxbfoam.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rzmjhklk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnropxz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3giijccti.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qamfigkz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sxnulpit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qorwjxsl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3stwhgenh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nqsbwoou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vgnkwfcg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vpnslgjx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcrkedy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqavcela.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tnfeuilh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zszwkhiy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3posrplys.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dazgawio.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xtomklve.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zxrzlvhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ychczxto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3engoexjm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3paddjmzn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmjnsr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3migsaiiq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sqgtorxo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfxlzh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hyslyscu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sejohylt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3whbauchh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zoivrzyz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3myzhfgao.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ahodungy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3inhlpyzg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gzvevprw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmmgyvn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3twtmcfha.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tihznfvj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cxqxhgih.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yhyufhqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gjgijqcg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pwirvyqq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hoopyrjy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jnmkvvov.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjvovdhs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnoqblh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ecnkrgpu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3resujalm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kfgznshe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nbmlshik.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wmslovnh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qkqxcgoe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfdada.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkqxwruf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ttznhari.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hnmmhghj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vawhenqa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vjglfzoh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jghpcmay.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tnyifrgt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3efcbvxxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3thtdbqfn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3delzsuni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ssambfyr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hnemoakz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rqohctbj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ielhpkzg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcdiizml.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvkjpqri.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwdvmwz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3abugfpco.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jhqktvbd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfxbmlyu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eegaybrl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hawoceij.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zzaiwuxp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dxkgywud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvqrzwpg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ivwmhxsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yraufgqb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcsizxak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3stgkimeh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqmzomgp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wafguklz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwwyvyr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhrkvnil.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bjpobcyb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oswspoes.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cyfwcnur.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ytnlcgjj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vrvbhblr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqvcjvor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zwwmwnmr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfntvsbo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlafug.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iseuxjal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ngroowjk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3muvnhlvj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qvivegul.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3loqxmgiz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nxylxwwl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sbkicbrg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gvmtkiti.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uodgofgd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlwthqq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhllbko.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tuofovkv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tqaazfnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nbkbgndt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vmetlbcn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3efrpdpyw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rscndryk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pkeljozl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nlchxdbh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fuidsqsr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qkqvdive.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xggguice.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pbjbvynr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnvqgpjm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrotzdmb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzhejutf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3enamehhf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tobecypw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzslchiv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omwfgmxx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gcffqawp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlhsezax.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwispmdp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjlsiptd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxykihxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hlyxrrvp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjxeyyc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgkxsvnq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhqesgbd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sgvznhir.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ajtjueak.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tuhjbgnm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gijetgdc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zthxetnp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3johdoutj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlfzgjd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jwjdyckk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3whoqasov.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mqpllrge.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3heizepin.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3pnwbwkzf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wlyqpxqj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fryyhfci.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gggvuvea.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aidihkwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pctheoap.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bwyzacsr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uclkmpyd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xeuygajq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwrsfa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dzgfsdcm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eiwzhsmk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bjscxrex.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sccoplnu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtqmbtwk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rumrxivt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rbkzyvdp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcasbxyx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgugqudg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avjvvwhh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlkktsjz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tiuugubd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwjykzip.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcwtflam.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsrwtozd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsielewm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdgtxspm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xdoseiyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofrjgsuc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhlbavvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwdpkaz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3khtsjgdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkylgjng.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zuogbdtx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gwoqhpjo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3izvbhjmk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cilerelc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3blztmoqq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lxadctfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dticmdnk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kyqojvoo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xujctbsj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kzxklobu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aymeecuc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tjsikzmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crsutrgl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hcufehsk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zvwykrgn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhwtudkr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nwbxmsgh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jerlykgm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcabjwek.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bmshfdjh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3coojksgy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucvwcocm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocesaddv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mnmggjqt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ohxsulym.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yzskelwa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdvfygml.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qhptcqdz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rotvcifb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3otcafjre.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugkbxrfe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gyvthavg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xxossolk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uphikalz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wzpbzuga.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gckxzruv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3imczoopi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3byldxhlc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3scvbjilz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hdyrtlsw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mnlhldru.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3byxptrkh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vfmfacui.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnvnnknp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znxokpcc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjgxpveu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jhwnecwj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bnfklcgt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fzutwlff.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dazbnkrp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dfkbkdvl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yonphnly.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pbyupfny.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbzmhypt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pajgvflv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3efajpomb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpawygiv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqilqghn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vflkybgo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lmvkxsgb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwitgxww.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mypzarui.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zywgptoq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gumnmvoy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kexqrhrc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3difcnutv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wnnoxhfi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fwfcxjhp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3idiwenbf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ylojalxt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pskrvtcn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zopctuif.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dmhodxce.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uuixabed.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vwhnpqga.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ghrzvhwm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rfyusdzw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jggvujvk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3irnnijgy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtfkyhmf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cehwhvxm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cszcbnmf.html


<!-- 参考信息 -->