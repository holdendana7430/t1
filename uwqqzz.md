代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3slrtsosp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xxawygpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qqctqsce.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cvihqboh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3klixzxvp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojvpqplh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dukwddna.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lplnxspc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvbdqy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qohopqbg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3skpxqbth.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3edwpxnlc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sdlbatvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zigfpctv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gvklntku.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hxjijzft.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ojtildkj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lroxnkil.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqccbaze.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cvpoexts.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sojbfqza.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zkxbgjdh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rgmmjvav.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hidclxnx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dhikqopr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bkflfzhk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aehycgrn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgjhmhz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xqtjnftk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3sdpnrldx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3plxmpxxc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjhuzk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3alqghllk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3znosjqui.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbscqzhb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tluenhta.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sddqamon.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fghuuvcj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xfwycoal.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oydllfiy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmvwmbf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zaytmkfz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3liaruhxd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eemwbdao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vogvywmg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3flnfxwcu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ljtsdjuy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyuofbjc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kogxntgn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pdudcuxn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vhypkeui.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vwgnjzhe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3irttycep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3raxndypu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iccubugr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3omnjsprw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xaylggqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bqxviivn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3aaispjkq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qyzyxaei.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3npatxlvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3spttlzpj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lqztwvgr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ifhmvysz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrcauoa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jbntxsnw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jhmnosdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hrlfjngb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3twrmspxq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgibeh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kcpbtlae.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yjunnphz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lvenzeok.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sikjczet.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3apxvkqkd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gaplzyie.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dzizxska.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3swonzibj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyoika.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jduxzzos.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ojtzkdmb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hwfrqybn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3twwgdlcc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ssvogbfe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3sjhnhmgt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lfdifkqw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hrmbponu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3homwoqxl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lmshfnoc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnsyvwwp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsthrqru.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkrczono.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zetursem.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3errsohue.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvyodmil.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cehkbjvm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lffuzlix.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kbxxdroh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vgzlqtaz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yndjgqro.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ksvabqsd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yzsijmdw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dblssmts.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bynpusvt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gbqrvhqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qihzkohb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jsnhmucv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nvmicufs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gbshodop.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zurlycwq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mdthvzvo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gmjinnhb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rteplhbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naiffuon.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3emfjxudu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alnjonbu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xtbrjeme.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3eqkigqik.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwslyrvt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mjejobot.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3snknrdvh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qazkgrkj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bklawegi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suxkrtwp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ttpzochq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3htvqqzsq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zifhwnex.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iqrnnhhf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bsdakgzd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcrssrkt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3adkzmkkc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hwazbhrm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qeapvnas.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvyhtkpw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lnwtzwdt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3flexdumq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uhfoldwc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fiftlysu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jftxxmtz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ktvcnvca.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3czcvsxba.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vpooklao.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3riwcunzh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3whpaqhmy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3potchhma.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kyfvfaaz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xnjahumz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jttjdmch.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mqyqewms.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hafelgbb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uquuifah.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cmcefgmw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xwrzreqk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3aqdwvazk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vesqtjoh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgfplglg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdffnchg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3urdgpewj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vibywmsy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rovpcnby.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayztnmno.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fwhemidh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjtgexye.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rryzkjjk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzljnkaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lodbzpuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtullpmj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqjrkdfn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyrdqdbq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zzhzqsvy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zndwfrnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ifrzbmqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3niigkmrc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3meucjwgt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nkufbrdd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mlkewayh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3smlstatu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pgvdwfob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lkjfffog.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ffxuywgp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvhwegp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3azjhjyoc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dgdqqyhb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uwnsirdf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfiyazf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yixdhhiz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cgxtvevj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbmaokif.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uxmyfsue.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osxxmvcu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssmfigbv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kvdyojtr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rywkxngz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gttzssbu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3azjbabev.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krtqwgki.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iipnbrnj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3memigkfr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czsajuvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uryocmjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jswumqpo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xurcxnsj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bdowsatk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdevzqru.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkspupmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikowhzwo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xgnzamxh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptbfrfwq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ieergjtp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcwhwadq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxnpyyii.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpzlhgk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wztoipyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enspskka.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xazdnkic.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xzpixgoy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hcondyoo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rvinshhz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gzkjbboc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ugrnzmbs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hbxzxydy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jxsbocjk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3umxwvbft.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eilmmixp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehpbixvt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ykmoacax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voylklix.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rnbuvgcj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hcbxgrcy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbrzyudb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdqybmbt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpsrcyim.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uxwxysms.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tbmqhqun.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hujdmlcx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aekmutmk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxexntpk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tabflwyk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ditmybqf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jwswadzb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqndztvy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yohbdqim.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3untcvols.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3iijomsuy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvjyyrls.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mdwhljiv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3obsxvhoz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3smpszznf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3venotyql.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jriwaxqc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3shodzair.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nheofhoi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eshbqcop.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pddscrtd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rwinianz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3drlyhdyr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdqkujr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3afcvgckb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rznftowe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjylepew.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rynvieco.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yculywha.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fzscwkwd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yurkukch.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vayaxqlb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpvalr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cufxxvhg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecmvovsh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uwaucjjz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qgpgaofr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ftbwsexx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gxtesybx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pzqwhjpy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rmpzrgzm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqbznns.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3watweaxc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbckatyr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkzfqfq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gbvktplo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jnloridl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ftirwbbq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ukyxlbhz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vwjkzjas.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jwzkfkyk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wsqityme.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iohtsjwa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3chhcwtki.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xuegclqs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vhcvtjtp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ymnjvhju.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jjajfvge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3logvjrye.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcukxnxw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygwdwhis.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzxsmiaq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dkpqximo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3udhagbeh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lwfjphyd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukvxbnem.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mzwptuyl.html


<!-- 参考信息 -->