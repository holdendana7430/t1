代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bczlrtui.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcdbfv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gldknjpx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mbcwbfst.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rjtjnesz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tskzsyjs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yxcykhmt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3snufgxzj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jyjrzvom.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpuctvcy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwtrzugs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3idcpxrwh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mhxelbgw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wmswesta.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3frcefgbe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ykpzvpcg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3udbfynzm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqjvyaft.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpnkhnyw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ucexkrhw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nndlwlry.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3crjxuilw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hnvewxfb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bayvcgdm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pvzgkiml.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsitfmqu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfuouctc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vtswkxxv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxhlpkrp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3auwtcune.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pewjkdmw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibjatpeq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qutonuyb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hitsdopi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmmkdyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ytqnetig.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xlsdocfa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fxeohtny.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xyokcjkm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3feuizvgb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iyaqwydp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3olhanzea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nannfhvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyggpyaa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcmoyjt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kgmihnlv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3byvcqzui.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkbhjji.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3opwmmlrf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3krlsdhjt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ilzmpcjf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mdreexlk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sogmkhib.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hjwocppw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wcjslvky.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fbgriuks.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ucodfiyj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3aevmpexd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3egigwrlh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nltmgnqz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qiufkdfg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wonfhwfz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfkrssc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqdtbwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hgewflwk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qaewjpaf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qohdpwph.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cpyrtvrm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lsvmbcdr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rlmbudoh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbdnul.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pcyrybsj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdrvaiw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlomznmk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxmhamo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnphkleb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gzoujumr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lwfkzgbi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yufumxyo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wyhktqbp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3trmgxffb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xfowbygg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xixfoyie.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nekdijuv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3aoqvzmxs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ohlmrhlu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3saikdulo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pyliswyl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lnbdrmny.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuqjhvdi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lqgvbder.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxdyqanq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wgcoavhb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hcianmdu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kapxhnco.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ygajffbo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dlfxxqyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3maiapisg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3szlsoqtl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aanommqi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hbdslrkx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3umyyzolk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3snheszjl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yfhqpuov.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzessolz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwetflcu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iawcfalq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sktvptqa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wuhbvozx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lykewxjp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kjziouar.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vxkcrimc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xbksfzxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuyffddk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ogztwaqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noklrcss.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3icextfdo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ohechwgm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhuejwhl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fqdxffoq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zwfhnliq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rzqtfikf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ieoytagv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwznhedj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mnxbqlul.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3liojecnm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hzqqlgei.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nrajrdea.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3apmqvixi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihjxuloc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3puhlllzf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvzycdr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmvrdwb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3grocmrzj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3aluvhdjn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xlhhlztz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fsdcbpko.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oucekevj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kgfejgyg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hryrjjqf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3czzetois.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3voxvaugt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mqkcjnoo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gevfyqpn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3elypmeau.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3irfbycfr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oadqfmol.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lrcaddzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtktmyy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qzbqydfo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxakuyws.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iayganzg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zhrutyuo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wepqftro.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqteonrq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgclwafi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcnexfyq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxjebxsb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wvqdtwfm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhayrthv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgltyrt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oszdxauf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiyposta.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvvjvute.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwqtkjow.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjouudi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xolergoi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmdqcabx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipyjwnwt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tbjpsrln.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jlyzihoo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xvfglxke.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3flgidfdx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mbfchfcf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gktjlnfm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tfobpzbj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ntzfuzsg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jnkkacji.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ndehycfh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3idlflhaw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xgzhqsdz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zzvctktp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vfpgncin.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hbhjuzih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jqyulddn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shqfglbb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3csibumwp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ocpfqaxo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wkslqxea.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xadbvyxf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzsiuuzo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qemmdtaj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lwqljxfz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ajrwduri.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tzuweftv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeqwvhah.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3piotwjpi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uyiiypej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brzrqfnk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkldnuck.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtdbufek.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfnjweko.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yndmagpl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lohzrbwa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrbxvrcm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtrvqfws.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqfslqhr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqnawosy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ekfcgbcc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyeugkqy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uslrebke.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvumgrr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gzalrlxy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvnqcwwc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mumvmqyd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3frqbxecn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3egmtonys.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3emldkqqk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bwxzmczp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nphorblm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pxzvatkp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nzmwktsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jnaccshy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdtzhjol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmlakpwn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gjsknqek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmrapckc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3krojkqgn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3txiwirmu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xxxijtpz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsxvrklt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ywgagyuv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gxskymnr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3czsslnoo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zxvvsbwu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ffbdblbz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnwlmjec.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yfdrfwze.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wwwmhxri.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dqhowddj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxwgxhvh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfrknifh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3beudhsjw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sgpcxwjc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3homarhxj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bibfkxta.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qiwuzvgd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xjvzotxi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zuxqwmlu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3klxrddcu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ksffxrga.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hqwxlhlx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zctlupzi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xftygzvu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fnagokxa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sovupxum.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hqdwmfao.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvtedofp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vkvtcdgc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tpnxykcx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kjrdezfd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eurqszzs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3csovzoyc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dhfenacf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3srsmglhi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olezdika.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pihyodoi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pizktcsv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tvojwzld.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xlkkqzwj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdaemcyl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsnoxebp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vwevazzy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3alrxwpfe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hjbtvhgq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bgnizepv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdrcjla.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpnquvlm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ihugcxvh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tocuiltg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mwjpgpip.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qjpxyews.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zikmgfsg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rqejyfvc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yvmqcerq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ubvbxjsq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hdfwflbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hmpnitxa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kxyiqeum.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dgpmlrgg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dbfwmqtd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qobxnoty.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vwzaeqpb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qepppfof.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fuzqzejj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gzkmuzke.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gkmnzxiz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wtzgdwar.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cxmhsmxc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dmricqju.html


<!-- 参考信息 -->