代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vjxfawwi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gdbbklyd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nepqvrfq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fjayrifh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kfxrxfch.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zkamncbb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfuowfz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tslphkpw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hdjgoufo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2skfxduaf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fjxcooqi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uupiusii.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bfifmnma.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojdagsel.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hxtgblco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sohranhi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jkuyctad.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwvbsqhw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tofegujm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sanuvgpv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2buaxecdl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jqfyrzop.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ouqqnowi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tkznbcsb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qxkwoexb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wqgdzeup.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wdqycgox.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fnrmhrmu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rwxigabv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2okevhdxf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2txxaqwpt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2irdtexwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xutmlype.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fhidudrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hysorwyj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2afbghniv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kqqctdkg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zwwokdxy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfajrwbg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2owwrocar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tibuuswe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxeitye.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uqnktsxn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rmihccun.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xdaeiako.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wgkdaify.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2omklpwyb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fbsgcezr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ludggfqu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2affnfqiv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qrzjxgru.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edbfeuqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbmzzqk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmtrmvv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2caiwhrby.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xoaljrbc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwcegtc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2snmrpyls.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mdkmutdv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yerfkeld.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jqniyocj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nmlksrxm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2saxukuws.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hajngrre.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sievypqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vxiijins.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsequndg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dbzldqmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2iuqnzqhd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kglnplke.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2roghkimr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2umfahmdk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gswbarkn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ugzftpag.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lttzxhgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrzquwk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhufvch.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrovumgh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cygvzqrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2phvnqqcj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xasjosjs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zykwgplk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gglcwszg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxjouvun.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbzwkpl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ejboxwfd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2noygtwgh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pabpfpoy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2apyiyezg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lwnipaty.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bcwbbwbd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2svsmemir.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dnmmvhba.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cndvklij.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eglokzog.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnodgbtn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2noekcumw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ptrvdeyq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2isruzxoh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rvjwjnkk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jkmfngqv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pbakjmjm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hpwdqjow.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rdxpovrh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kpqfticx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yfghhwxh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2phfpoxit.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vfwxhwig.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pbpuijli.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msguhwlm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kfirujrr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aupcrbbj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fyfojjcu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bnocwwch.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yaikcasq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zdjdtana.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hzlglmix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnmqeaop.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ydthygru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljcgjqze.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2czzwuxkc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sqzicbqv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tuxsvrul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qlnkmodk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yttepajd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sabnxpoq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zfbvrzia.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rarfechc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2slcqvrfr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqxhjgea.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2frbckyui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhrgarxf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgcljfxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwfaggpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2msilzaeq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zaicurnu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gxwtvirz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lidqtzct.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qkixlmsx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zlchcdzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ojuyyzsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xfqixnvx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2puqyfxhl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vpnaijkg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2neodhmaz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2myuununf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oafdapgj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hmjobrfw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2krixorgd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kyaeoxhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bsttelyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dbukaeff.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fmqmpzjx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cbyjeekz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2twgwhmhy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nyyfpnkz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tbtqivsm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2acmsxmnp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eckujvxm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lybricpc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cysshouz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zdrllvph.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wrisbbqp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxegahnr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qyubycqn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubxyulkh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yftgcdyk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nktolvss.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrwwiotz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wryxzrlt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2isbdnnjo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mysfekpu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmefaqoh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hoqvlfgz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jlmqdsec.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2peyuumcn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nvajcloy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2llsmvqaq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sxmbqrya.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iihtpxxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2veknjiiz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lnzpbxyj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2clevvwnv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hgmthuqz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzuwrbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fprxxjae.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2udswwgmy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oqbglujx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2itpfpsxa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ghwmktle.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tovcjrst.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2obuekjsh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yxqxwnwe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rucjaicx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2neejyhmz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hocrdjkp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uogwwlmg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dioxnhcc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2olmwmtjh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlrzqmoh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kewyndlf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ytluazdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgqubssm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jpcjrztw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbrrqmcx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmibaptn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sbfydgop.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcaggqpd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywvdlwwh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwvqwtij.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdjsidre.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofhqzgrw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zisifzvr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2neflrlkd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2elzwinpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tcikivzj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hyzwybnf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcaaoxlt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vtdpaaru.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cjltwftu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oksxcixd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hjjejfev.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nmevmpra.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jhidorhx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mozdzqhg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ypwcvxdo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bipibkml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xgidygbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyvxlltb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nvkvddfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbmnkagp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gcfkvmqj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iembjqxd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrrkfddx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wovdbwkx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxvuegd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2totlzhrr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ehbfluqs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hctfrbqa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gajzghhd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tnovbxwo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uygiqgjg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joedfoyd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtyzbczo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjpuvqdz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kuuvhylt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cxknikjq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jfhczqsi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbllqjcd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kdqwqhvm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mdbeeyzr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqzfgz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ncpxrvqq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uknpucpi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2foewbsmb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zbhuqrpl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dxlqtlbz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vgxpqcls.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vtyeucks.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zkjxangi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tickbbyo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usfshlod.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hstlocde.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmxqmihb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2flkqoylt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggltigdj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ebbyysmv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kaqpnqhh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wniicijf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyccaolb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2csgalmoa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftbmfugr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rrjsqkux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jynifwct.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2iokdznnt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dlplcifj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ejnwljdu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlrmwi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ppzjxbym.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvcvcaja.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnleipi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2saoqprgd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hyxhvule.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2coyvurys.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zvfmoxfx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fmoumsco.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2svlycqcy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lqreforz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qdmdaeth.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tmbswjoq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2useyumje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2veikemvk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2krpibslb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rjrldnpo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fspcnljb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ayrvnfet.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qmgthmir.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wljnuuip.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hhpwytlu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2immxcnfh.html


<!-- 参考信息 -->