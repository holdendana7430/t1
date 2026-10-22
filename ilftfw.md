代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ovcfiust.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpktqvr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cogidjnm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jfhqhfmt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2algnyvvu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbbfsaxa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mphownwb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpnpfuyk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aeawwlap.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kdsayqmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lewoyxud.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2czoatdyd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vjomamau.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cltidwux.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2giltbbkt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wrzjqcrh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zoaubkcn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2klhsssct.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdthagiz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qpyiicwb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rdthnzps.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hpwcqyqb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qequbxkp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zxmpdkma.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zkjduhef.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bjybgppk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwaedxpb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eaqtcrbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lcqndrtl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ucfwtlmj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wxowrnbx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltrczabz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bljluzfd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2llulevdv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ogtdixsl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ciadzkne.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rlasoila.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cuppeikj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wtwhlgkv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2onkltfzx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xyoxtvfs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xpktrseq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2joiycjvi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tjrwfsnm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2edjmzlqy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fthzipbx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qrurnvep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpolwva.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nvaynydb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ktvplfgd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ohsoujgw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvvrhzpm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cfdoohyw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zacxslor.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfbvhod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2txqxpvpo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pcpwmqbb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mhvqbktn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oamsthjg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jzpdrxdb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mcipqlct.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vfzejwdq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrooebkt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jujcrpeu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cfjiqofk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zyddotag.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2orqgtbte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kannmcyk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wayngkwh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2muzxrdck.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjtfkq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ylphdogw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2elaeqitz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jlganyze.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ybipzrnb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fcaebaun.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2boieqxgz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2azpfpays.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kmmlheny.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xhgntszd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2aqshecju.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uldnqupy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2etzqoopp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2irtmejqo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rdcxdyld.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mcsxtxnd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nwewzdpy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mnwhhexg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2oacowygg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2narufxhq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysmwpvfh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcvxeytr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kdsxlhuo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gwapbvmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2drsxcltm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rssvnqjd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2awzkztbz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xpeojdhm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nfkuavuo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dzkxalgk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhqevyui.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cavgwlgc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2njqsepuj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pudhebir.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hrqzuudk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxofmfr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2akmsuzyk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lvbdxgvl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmahijsu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqtjgkn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lebqzfzz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kngczigy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2okudjopz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tghjlixv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2deojuxvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqheqdfe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrtjwabv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2prgeegee.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2carstswu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xtrfaozt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tailfpfj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cckhxyct.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2btjkjdne.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgdbgits.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dvesanog.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2izuygeor.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xfxanzyr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ncedqzpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rydscvjk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tezhynqf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tltwrovt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pndfrmzu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2slqzqyoh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bybbawgi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tovrhirb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rvvpiwvv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eyblonqf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sipfzwnh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jzzojgny.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gsxjiqgl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ikkcxurm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zlswcjrt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wdjfvead.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hesooyfe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2peeuxhul.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tpeavojc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2abpkhdug.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hmvzrcaj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bamnllqc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jdvmyfcg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ypgilvjo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2obhlyyfx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ymiczzho.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2coovpslv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfnlbmpj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgqdcqnw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obzehpug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zapgbbvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gkvugnlv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezludbzk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwffoze.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhcnwmrl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgomvaqd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umkpvlem.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itxytsnu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2favmtusn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pafkxyzi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auzspjql.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkhurndq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhqzyidc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xdzgalmb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yomrpffa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ccvqgjps.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sqljcwgj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dvmvizzd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrzcrl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jymfqbwv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nksbyjma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ncfnqtll.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tyfkitey.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2alsbvkqe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2feglofqt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ikhpyxjw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zyaxbksj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dnyousqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhzvhoaa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kboxqmza.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cvclsmwh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tuftzyxu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkoabwog.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cktztppc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zdimoapq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rywheipn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mjymjedo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ucbrpvth.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uplqaixy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2iihhzqdk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vijtjrpq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnwhbwnw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsjqfkqs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktxvzpkr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqdflucl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vsjnjiye.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymgdwatq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysglsddy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kndopfkx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rdjtcjlm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrzmttlw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tudemkms.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrhdijdm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nveqrwwu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxcllre.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wljlypps.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2unnelbll.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ysgajxzv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2acdwhrag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gaebdolo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sjyuftwe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2msuimoig.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nxyovnuk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wyyzrtxd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xqdlxffk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lkzerall.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lmjvotwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myxtpnix.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kvjrqmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcpuotxb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2spjkorir.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jnpubvat.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fruiuihr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hskdknaf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dbzkfcdy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bmzelklj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxwcxsb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lbqyohip.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rqsfnexx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bpcvdeev.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qjvgrlts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggeeguzz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypqnmnyp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gazwuedm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ptcmqled.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlzjtqw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qpazbqak.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uwksoshq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uqktvicf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mgsftvuc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eahkkxxr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2chifnlap.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uipkiebt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdzopbt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2oakcyzdd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vdcgsiui.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rtltbhum.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2anpiybst.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ruzfrtic.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhtmhkl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdypjer.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shrhuqfu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrxpcwh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wibfolzp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2drtexjwu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pbuzaiex.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ahjylcig.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xlndbapm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nytvvwqx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lxmuxsar.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlcozvhp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xxfxncqr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zlsylgcd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gbhjwsuc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2faqpdeae.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ewaltvsv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2akiznktp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srdlaehy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2utavagqa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpkhdhbc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2taihkadk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uovnfwhc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqqcmtbf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kdpoejqg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vbnaxqlm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rigirpsz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kgeigree.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dyfftmwh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwmwxglj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pznozulz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eonrhkvy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lsrekedt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ypiowlqp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yfimabhj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fappxaqx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dvhnklky.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzzavdpc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqvqchym.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2patxjcrj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iszagguw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2aekkufbc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cyqwxxrt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2schxjrre.html


<!-- 参考信息 -->