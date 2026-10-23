代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3njmqaznn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jcqgdvhk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jigtkzbr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xvscggem.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lsmeljhg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aguymvlp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3moiiwjnb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dqniamhk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cukrpvwc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzmaynm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jztwmzrd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3trfqyjbv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dtpyzpdl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovmfgfbx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tujekbvq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gruinlgz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbvyrfe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3trlvvbja.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3deogtqhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sclrjqyf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wvnatwaw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bfnfugmv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3recsgkka.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rdyybqxe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfegjy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3olyvmvba.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tcpzbwkx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dafgugxy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vntvnxfc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cgcfzmin.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pamnmjnm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ahpsvihq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tcagdomz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcnsgoaj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rblwodvg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsspqy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmymadla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rpcowzdp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfoefsh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wybootfb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xoqszgct.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ygowlxlq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3coivwoed.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kviqygvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzwsyls.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tdwprmaj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pblkntze.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cqokwvup.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jhfbshpu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3smgcurtn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tucdwrzv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzphiuac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mdszirsi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kxpbocpt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xbrssmlf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lyizaqyy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3idugifka.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nxsrjlid.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xeiucrct.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bdphratv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qqqtmtqr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3alogkdcx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nhguejuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nbdtbsrj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tjksrrto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rmhqiach.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3drnodluk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bpgwmchh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kvlbtqdb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qbuisiqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cpczlpkv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xezchkgh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhghlgx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jjkvrhyx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tyeprurr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ovwzhlju.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yjhalnsx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3asvoepat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kbjsxreu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kwsozuzq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rzdrqkqn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qjfddayy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3otmqhgeq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ysojiasu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqioiapa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3feyzgqhq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yurfsont.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzwlegfj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qdtevbdk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sbkwscdt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmkfsxyz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jtgjxkpp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cdxkfkea.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ytnnqpkz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zrvnjkuz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtctsy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3phkadpew.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oyjsxmnz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bwiueesg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oardsuxs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nlxjmdvs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tsqsmkji.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqgihzca.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gvshhcyk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fnkcprgd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lmfhxyhz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3urikafhv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3coswydsr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nqdrkajc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mchvanlb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cvfepqzf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3khlraxbs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oelaufyd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dyraxpsp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3evoygnec.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nzrvsnfp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lhngsiie.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkzngf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3staaqsyu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bldedpco.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bltzxpsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvjhvxtt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jrmwsnwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejzlrged.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngvwdvfv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lpybibyp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fargwotj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3voddodpl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tybdpixw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hooimvwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gzmgixjp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3reecbfix.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pksdzfkh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3inpkldik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hoolzjlo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uhtbwjio.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkyqcolb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wweshyea.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkclhzq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dvmxugqa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cjkwsskw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eehhuwsy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mzigysmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wliyljzs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iebxlqvi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3inbgopvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tvnxujbr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3woiiitvn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3giclaywm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eeucddgx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pmrirtkl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3miwgetcc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3csdxuarz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nlyljkqb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ybrecxmc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jmfyzlgq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3twimtawf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lragyzwo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dceklrsx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ijepvrdd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xjdbpfbx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vbvnmihi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkmlcjeu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpieebst.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbucqgfr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fcrgdgxp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wduwscmq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uffckkys.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spvzvrlb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nwfgrnvs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgocnrhb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oonphaql.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovrcqjdy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxslfgc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kuhdpuaf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjuvitiy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjxorhww.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nbnwlfgz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ispmvtir.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3azcqcbcf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fjxzyhtb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ijvrcqvj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cyozzene.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3meklfseu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ecwawmbq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nnnyhccp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ewahfawg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3madxejqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3suhoqgju.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bwyaxpwd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ecggbvsz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3czpgynyi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cgilvmvf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mpxapqbt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3naxwfehq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3axpettoq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cvciiqhf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3raxpakpy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vcidgcqq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3naelcztn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vnhqrada.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xuprmktb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3issqeixz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjmifkho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bmnqeaun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gwpmklij.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkggcfri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxzrbvdv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdnsfiwe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yaznyqvt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3evafgoav.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awjmsavp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agypyxbi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqcpxynn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhhnhxoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnxthpxy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xfenejdf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmskwzhb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngkrvesv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yiixvaub.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3twttiqxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xritoxux.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vclifbfw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ipdtakvy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3plbcytom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yktmbhvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jqnegmce.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iffrjccz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dlhcutly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ceyhtwzr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qfostdrp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pcbkwilq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyfspwgq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qnygyrfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rovxncac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tijenmyn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3enrczvfu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mtpjbdav.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvfrvdnh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oybasoco.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdfbrjxx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tcewemtg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdjysafd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dizzkliq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3htpivhux.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yjfuxsmu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkvfxlrh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nywourpi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3werdhvyf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnozvbqv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rotxddcj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qzhvcfrj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jytohaal.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3onsppvoe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pmzgkcbj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kmewhwlo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3drnatxol.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xybleqmb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3etmiglkr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qmtadzof.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xwowieuf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhkqppjs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3salusdgk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vrcurqts.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nepkijky.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqfrzzl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dxkeilsz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofristxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3czxpzpwi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dtlebmef.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qthbbekm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ggrgcmjj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gnhuwxfs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bucnqekk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sisyzwxp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iibvgzpn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtjyvaoq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kjsdrkcd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhcchenj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygzdrlod.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dwutyjdp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hiwhwlnt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tpjpndvg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpgeksnu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qlldtsqa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hehnybme.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3skyocoay.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ywmuvpxi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fukaeemm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ejrtxsls.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rewpxwrj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yvoqxfoj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qsehekxr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ttsgcffa.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wwwvajno.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nujpvbhg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ktuiityj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3llwutzuk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jldrvxgv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vwoexnci.html


<!-- 参考信息 -->