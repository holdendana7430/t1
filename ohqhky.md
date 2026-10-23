代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3unpxkquj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3voewkzda.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qfsavgtf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3urcnudsw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qxkttvad.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3suhoevkm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3muovoofz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3asyqbufs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ydmnnxme.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hemfyckc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bnaglksu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ufsvataa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sitfhsne.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nduovhyi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hrdztlts.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyqitnnw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vkfieqpf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fmugslmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zubcpbib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dfuvwgrc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zhfbdrxf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nahjsbgw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qkeguohy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ohevyets.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vnugfcmk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rcvjldzl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ryzmkgtm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lwndgdtu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oifayyct.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bzbwhckh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rrfexerr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adrdafrr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpythdn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3myzjgnbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vvldnmfr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqkzcvqy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpklkjwz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uyhhvyfh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3aeptxubs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cgygmldg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3owesdsyd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sgroqucy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbncrgyk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zxvkbovx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vfvahjzi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmdteqw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3utafnsxh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3aapbijsv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhmfqpp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tbyisnaf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jeqalzwy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbohvzub.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3scfrolqr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jipaayvp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vupschwz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3asekamnh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xoljgjcm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3whvvtfvb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qzszxzeg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpinrytj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vnplhnrh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3helwmzax.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbnziw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nudsjskq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ursreqkt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wkwwylwg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dxepwtww.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3stcbhgww.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uitxditu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpckjhib.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jmtsojbu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kymuxltr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3atmclocf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mdznsxcz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hjdgqjey.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ujvrlghg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3aajldlwy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ccxufsmo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rgajzfbo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ofxxezhk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nauvxjvh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbdtrlt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nidnjzgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3umwlexku.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qzaazjre.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rltjmpkb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jekshhfn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zsiciygz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3twjlbrwl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uoaotvaq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uaqgsdun.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ieryqzvs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpvvpz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ieazrqiy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nwvvsimp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vvruzcma.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vlfqlgfn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wppjwaji.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzgzrtuv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppirhahl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3npuquzua.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ngbnkjor.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rxwjmups.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xlsaugpr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xuweomwp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wkeptydw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yjpoijun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zuwlwdcc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3optxsvbv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xutpzndr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3etlwydqi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ejntvowx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ekikgtnm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3msrewgiu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qlyeeczb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3athtbswe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rvdutsew.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xgqoneyj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cqgtpzby.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fdypcheg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gaekaqss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvaubicc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3onanmzqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kymkjxwh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wnyyqtao.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ysdbckdh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dwkbdrgd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sbraroqn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hozzxuks.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tpvxpatu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3juncjrkq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnvozjqh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhbkzijd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zifrvaql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zhrnuszm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbhyckm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyblmyru.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pwwipvyt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3urffmyex.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3neidonwl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3skppyopp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rudubkpr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3smqjgmxq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3deaztguu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3artplezn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fgiezwcw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uogphvwi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3luiunntn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fuqwqvcw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3merhsjbm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hvmgdkyo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mkcrgatk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrlvizs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3moomepha.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ileucwae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnufehgx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kiacueww.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fypegbnr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yrxgrlle.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hjhcfkmf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xjpycenv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tyonhnql.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tnhoirua.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yiqpyphx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjrzfgxm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwqthyyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cvatyfsn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdeulytv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aloitjiu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyzlsmbo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sybalmys.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3biowuffe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciiuario.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlkrwgnz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrfcgaqp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wojdsuba.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrwljwuu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhfpxrgq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jsnbsjsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lrljysme.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3csdxtjsp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qllwgqia.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ceajtqnl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdpnasgo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkjmzzf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kzlrpbid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xlvrnxum.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yazehrdx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ccjdbkjw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdclbvl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3juikbitd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cdalsyhh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nuwqpisb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nioaxsca.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pqpakbmt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vtkjckzi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fdeobuhm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3giciyzpe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfxoiqzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cdslllnk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ubcilbos.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ikgihyrc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fceigzcl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylqcffhp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hdlxnqan.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ryxxwhoe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gaailynm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uffwpscj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vulvpdpo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jobtnxyj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3whkgyuuc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdhiiwyt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3habgrjqh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwzyejsb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hqbvizlk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3howkuugw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycnkipen.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3brlhrrie.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eydcasmh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3agwwlwrn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nurbkhjc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lotjgqew.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ikwmwrty.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tsczjnbp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uiwecuoc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3afzcgtyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mozxztvu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zwjtvsyb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qzrunssl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tfmwksfy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xwcyylma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hajfuygt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdcxplfm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pxnboafh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnwiagwv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rmpoicoq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wjxdoomr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etqsbjeg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgotfgzr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtqkwcp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dqpzrlof.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oeakqguv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3phyycado.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3acjpufzd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqmsoysq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3aynkwwpw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ddfkortq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okipjxxj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlhpqxgk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bwbxvvyn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vdgcdorp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3spxlwiar.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhzfmmzb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lwauzned.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uqdpslid.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xspbstox.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cuiapaho.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3exqjtecd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3brdpdwgk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tjdnnifp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ubkqkvcs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evwhmokn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mokozmgz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qqwtvowc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrmpqkfn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrsgpixs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yjqogckm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kvjjxoaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yciwrnnl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhoonk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qxovtaoy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3skhrnmdp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hhgabhlb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qjdznqjt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swwrprmk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbjnzlwo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpugcdpb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gpklabea.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvxpdkod.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mbwpthug.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bxrqqymz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ozopxqmv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cculjvel.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3btscqwwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjygipil.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsbbnlkh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nwoucxfc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pendkfdg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zryumzrg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tttjaqyq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3crtilwog.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxxopw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iglcxpwy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xeguixba.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ewfvumvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3oxnqaokf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xewnlzwo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zapcrjfo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gqwwxpni.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mimdkhgy.html


<!-- 参考信息 -->