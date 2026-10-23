代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ggautzjr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dnupjoim.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gwqbcnjg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3salpufbu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zwovmqsk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3txictjms.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wwegevcq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wqtxbeoe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mlrywyqw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nkdzxexn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eaapytod.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbssozbh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vjwfgecx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ngbwmzri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qjikmvrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jundwtry.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hvgkphde.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vgssbtvw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fqooaiot.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3crmgsexz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rcwmzapr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpyhotbn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3otkibsbu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bpdibido.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hevipimd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ttvqvwtl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dtgyfyjv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tsbnrfsh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lynlkukl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xftylfqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tkehmyaz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qctnneuf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifjapzhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bvbdiyvw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qiwxtjwe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pycmuytl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dtgrhcrv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jznjdpyk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xfcrstpo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jwizpkpj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfhfygh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ntchvbpd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zhrhqgtx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nquyqsmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3okqqduhs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wuuxmwan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yaaspcgg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbvkswu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3shijlosd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ascqxvbj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nvaqfnwn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irpolipb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ctxmalaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arnslujp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3llfexjhb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ayvzyxgj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwepuiy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hohcfjro.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oiqctgtz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3osysvwyr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zxuzqczg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ujmgqwfl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mkeircwy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lsrxgefu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3idodlhyn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vnuwgxej.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rtvkfnyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smnqihya.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfzrwf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3csyrrmgz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ssbzpfzu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3iaugcion.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qdmbimnd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mwppnrch.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cfiburwi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mepwnljt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kqaihqdl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wvovwjun.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kiqdwset.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gpvfptwl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xalfddxl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3voyjqldd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3usngqgsx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3detqslvj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jtpejikp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mdnzsbxl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqzhbhed.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gzlyjzfu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nmyfrfto.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dutfgkme.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ikfntcfx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tairegih.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rjdqmglq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3loccapey.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hhkotbqp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlpkhsbq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jbxvouuq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vtwozirq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glqirydi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zfnmmzri.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bowfgpwk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3angbueuu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dbwlmlia.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzamssfy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cspdnsqz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qyyyhfwb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xouqtdtm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ndzzmrri.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mlxbpsxf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amigviii.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ypndabuo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdaigjtp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sbzuzghf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vzuidhjt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vmugglfg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qgkxmzxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jsqirrye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnsmlqfh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qpgedbwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szrpfebp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wqrwddiq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gvdmrase.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tedadaxx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kqthiihh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vgevbqjp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gbnlqqjj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tcvingji.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uobqpirp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yotspyhz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hziypjsb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iyjrwyrx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbsgyox.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzdlruej.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cozjufzf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fjmgvhem.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zeywbcbk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3irwxoaoj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lcphffuq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3klqebdhi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vuaqhhwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fjzdfvsp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pguejrcy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rkioztxv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bpanafsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gzvpdzhd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aiawloau.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qyznhwni.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3auqwvtab.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ydubulhd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dekucsks.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cmcsrfne.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ozmozaax.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3adsooebr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3krhmpxvu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vxfubgsd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zoccigbb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tmfaonqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sslzdxsx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hagmondi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdxdmfmv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttqzhfdh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwynzaxa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lqgnuppr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpdagleg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvrowyld.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3iszezieq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swgwwhbz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgwrimix.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txafhlbs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qthuodxk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gzaacqzf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjznljwa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmkjumkt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gkieqqmn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vtldehbk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mkdgvpwj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gqhylcjr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3buozgqez.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wyjqtxkm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ejjfxtua.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qlndhpsa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lpdjdjac.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kzhwpksr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rfuardfx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ozsfsmxa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxiiubpp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3edixdrbq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hagnrite.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oprhocir.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3emrydgzt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3seoptloj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwwvqnxf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3peomlfiq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbdxevin.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljvlggew.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rpcnawmp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bavnfsjt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mcowmtwa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xstgdmix.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgkyxxvu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3evkdjmvc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ougffung.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxxnqwqr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlpxthox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyztslix.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddlrvoyp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3damaonhu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzjxioyv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hggkqwat.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpboclle.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gntfkgzg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atenwnvq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xllcuska.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zptqxwxs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvngwxuj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hnxnafrv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3txurnrsf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqefdwzy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xbwaylvp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3grklvyyl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tsatmfmv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xgxnczaz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hkbjsgzk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3npmuepjs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mfngfhwe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tzvcxbwl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3afyvujmb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kevynhuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekevqhiq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ddqxcajv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moorwvgg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wqmssgvm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ohgfgocv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zdqottoz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ycmneoco.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3htllbxnf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yacgghgo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3evjavalj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehmneubb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3npeouazs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xfqrtiuc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hjyvctov.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qudplsxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3swccqntt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vcfuubwu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxakycuw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tvftzjrf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsnzrfzr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xbxkuudd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ixeefrrm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mocgwios.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3isigqcjn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jmhjymaz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mzexeyot.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vsehugba.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vshvmmgi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3slfcnjpf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qalkbcpv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3omjgrbob.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xokcnrdh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elbmhvyp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3igmvgzrp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xqgidnjc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iikntwix.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrmqhal.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjhdgnwn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zgobxzsy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3eggbnpgy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zxcfdcou.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcjdddai.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqqvnaco.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzaffamz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lntruytr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yhhauwcp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gihnovwy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hfwfqfnu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jjqdobva.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cawnbrdc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hibtvitu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uasxdkkt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkwywua.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kffrayne.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ppifdavf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qaceqygy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wsxtfniz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3aggbxbjs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dvxgimgo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nzgdkboa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xpjezguz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ipccwmgu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aqzmadqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ivbwupii.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ecdcalkb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hiywhcsu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rmfnlpgk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jrjtvehi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3arvtqjya.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bysazejj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3almeadff.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kgeppkui.html


<!-- 参考信息 -->