代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3somshobj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lhprxbfk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3efxjwhnd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ghcakddz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfufbxvh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3svcwdbxk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jlhvemnl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cogpxqfc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wyglzsxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3imnbssjn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3syrubfjv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wrjcaddo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kiblivny.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ylirjwch.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zqhohruy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhhqper.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygfqcxhe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjwmzxo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzoehjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uszkgznj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3pxufpkgs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nxvvvsia.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3abqfzqod.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vcvkqmiu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dqaatbqu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtxtnvu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bimocvir.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dknnowqa.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjdwli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ziqacela.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dpvwpfnp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jtinpkgv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vlesoeay.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bfnkmfaz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3avdbstpg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xjjorotb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qnsytzgs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjkyqit.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cbubdqit.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jxrafqlk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vdbkotwu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3srmhyrjc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hilydjkr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jrsagzzl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3btzaijwx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eqblsuxb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyzcsnl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kbgsotji.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ydbxcqea.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3csgqzjnv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ledkwfbo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3prwptmpv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yhorkxpv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kxndwqqg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yfmkmaea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tuhphugu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zmanzvsj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sbfcwpym.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hebaztfe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shmxnkev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gkeozuxb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wlwyhylq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pjraxirv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhrpyxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mixdszyt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vuwwkdik.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3svcgqiqn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejizppmw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mirxflss.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zgeckdlm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yyttmykt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dqbizejl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wmbajkto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ihoajban.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pglcvenh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zsbrsdav.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3egqqzzmz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wgyfzwkh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mqgkhmav.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ggknvbpl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3latiqrvt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3avkpkeel.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yxcmjsrd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqddgh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jowdykjw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3semhskzu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mduuidnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3adpwuwfh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3svttyjpw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qyykqbvl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sboqxxgb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jsrcvffp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnejtjlc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ioznozzk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pfcqimdf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iltpayeo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxjtqjm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ogubtrqa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ozvyhgcc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vdirebbn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zcpwezlm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3urhpeczp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hqhelktu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rjbysucd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vsrvtlws.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3febjcjcj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qpowtheq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfocknjn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilyhcmod.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zfvmojni.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kffrpxxw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dcnazqll.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nqrtcyrn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nxgiprek.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mutsyysb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3imrfaxhy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kyehwkug.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ncpahbgk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3leotvyxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fcqzcnvi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vsxogqna.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awogdyro.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xwgpmkuf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gyavwymg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bpjkfwuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bbaghboy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ifyftnrb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gpscqrhr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nzlndjug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwayjzsw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rszlflgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkdsssuz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkgqqrtj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kkwjcdav.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xstafmuc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xccguydh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ijxwykpz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bonlopmg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ytclxcrk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymvbixhj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pzuzvhtb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mzbowlgx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3acfokqew.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yocnnohk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqkvczhw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suyiodlf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mratekcw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dkihofkk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3skflnwns.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iasfjvmn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mkrdvbdf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qbhitwin.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yqelcfqp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3otrjiytr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3erfxqwjm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gxuctaby.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3maqdyuyo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yslajjpn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kyyhptfj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubvxgbay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eqqfmwyt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ftzmlcvx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fqkkuqrr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3evzpxspq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wehohnzd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3exbhnotf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hddbhrrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wfzsmwgq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vxnybveu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3suadiwea.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mbdpfjts.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vngufnfv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgjfbltg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rryznkak.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgthuvn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrsoys.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubbhetmn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ssbdhngm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtzhzqnl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hupygshw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hpoikenp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzkrmfsu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydwlmpds.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulcmyprj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llfhfjng.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrxoaqyt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bylngivf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oivdzhrg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ybuhhnnt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gvdiinvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3crisgxgz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwmkxvgw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dlsfldto.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3aghhontf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zftyukhu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qlkzfyto.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3imdbisjb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtlmyleh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3inhifwnv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gipamwwl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxxtndz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bmwcqutl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3actmsmuk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kvxmfnxj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mtndplhk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqtsxjca.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cnnsndpn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3euetinnr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jkkaqwnh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nyscpmvb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ngbnkjjy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbjrpdgn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3txsfomfd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gfqfyhtu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnzyhukx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehjxquuy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ormqvsqb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqpyhumw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qdngptyx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vahbkjnb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guslddgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibacqyea.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jmdhzueg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdcqhfuc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hmrjccrb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmnfuufp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgjirntj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yqgjoyha.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xuboalht.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yahsbefp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rkjiaiyr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hiibcisa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kevxekcc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3artgoxyj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3krnljczj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3imkfisnq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3urwxfjrr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gbdskrpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jnbxzwog.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nzjnnuur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqvmkykm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qhiodhhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrjpqrtd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3blisnzmn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtmnjyyj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3svmgmyaf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljkxdbfb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvmxtkje.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gistkpyd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fojwynft.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcqarflk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hccgcpvh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3buhmqrqa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fnmjitzp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srnhrjgj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vevnnpit.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gepmdacc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vijfrhmc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tbqfuqxj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kdxykijr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwatchzy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wuqbohkh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tevgtvbe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gofkdard.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3himxfspw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wokizjey.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3quyqueuc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kcvzylms.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lccemdjk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xuugabka.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qcyeynaw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vocnkwdm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ejpzkwbp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gpypvodj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xgojmpcv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbqwfxrr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqxzqftv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohxlkldh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xctltacp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3albksdds.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hgoqoddh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpadmmqb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyhpqfis.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pxsnxzvv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qidrdhhc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fsrnpkft.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmhomfnh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pxqzihwc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zuimblwt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3plxqeeug.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmivkaqf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tjzbryoz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vmhteash.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cacjqmga.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3codhkuah.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fepfgmkd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ylhofhfj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pnrjoegx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ewtxgvrj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wccmnpbo.html


<!-- 参考信息 -->