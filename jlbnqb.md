代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rzyodywf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vsxdhcpy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tyddzqec.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kniyxzvk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3agefspei.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lajxpjfv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juqvfvmn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3udamsuzy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bvqviocy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkshqwql.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oplrjiwf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3owqotqsk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sapzwood.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rfxerces.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gyzelpsd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rrvahvst.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qaitqxas.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dxvdychk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ojkkovoh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xddjorow.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kuvwvgrz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gneugaml.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwtjnkgn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dpvuvqqa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3baisutzv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xkzvqnuj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vnyxoiqc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hylfdevw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3clnqcbbz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufisholc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qdicxbqu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3opinenco.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdbbhmns.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vrkrhyqq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pwffeoln.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwyryapa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3veoskqwy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tqbdetpo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lpexezua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ecimmhqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rephcgvm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fmeklgqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cbatiuxe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzotqicy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3byzvnjdv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vylmhngq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbonqzg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ylgrducz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqlrxui.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3paogdavc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gedszlis.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sodrjzfr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjqklwz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpkfina.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3shaenmex.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yhulrkcd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dbfzzgci.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rqabwkiu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvjwyyod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3shoaldfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kdhcwdkt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wcbdfiqn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bxsshsey.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3svekisgn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtkiqhk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvskmpog.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ogvhkwbz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pddzcvmu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpnnoto.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lxyhraxs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xbkcjkob.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dbiauqbq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hpbmaefu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fqpkoboo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vcnznhdl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wsizkbum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zlurkmzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qdjvmbrd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxmbhwi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvacyfrl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3llpemlby.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ijswsomj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fvvedzpf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xdsisoga.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wimyhlqr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pctddwlh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yrddsuyu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zynobnmx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qmejqkjw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3adgfwgbh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wdfqabui.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hafqumhq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ppsidlbh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bnshbiof.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3onzdjwkq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llegquvl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cijmpjjc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ymnprvwo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3obedqusb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nxjpjduk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yaslxcjp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zifxqmer.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cmsreohr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sozutlpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bnrfjyxx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3liglpqdi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ogcotnzz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3teqyhfzy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jnizrmyo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tgedazqu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kdmbtxff.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wydktjor.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpowslcm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3olaieiul.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3texqlpvg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3puxfrvok.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ieccutqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsnockwm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ygxrmjxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oityloft.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlebcusp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gnycbdba.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uyefhgxw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nhpttvlj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pivagsuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxgskcga.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qyiasjah.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trzkhdym.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lebvweqz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ektrbegd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3llbsvlwr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eupxieuh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sxzywqhp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmzizwyc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uynkybei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3afwahuhv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhutvgl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3biotrrrr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3evynchlq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3njaztfdd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vnnsbpem.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3knuwwppk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rldvviac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjlgdoq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dthdnctk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzrqmhl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nrxesldt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kevxqmuu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kaxrvejd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3elyywzgy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3avuglidx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aeidivka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3louxqjfr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dfwytojt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ylxhrrzv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3opguuauc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cylcorcm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vwtxsnld.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fucjdxdw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdetly.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwbpvpqa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3stensuei.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dkqnlgyo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkzgnefp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aknfijqz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tvwycawk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgiqjtzt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3myapfuvv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnmiudj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fltyonxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqryyd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njldkqhc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcjcsgwo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nkussugt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dyxrrktj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3crizptjx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3urwkglha.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3istaxwdt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ckacfkgg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qmorstja.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3awgkszdk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yppidyxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mtqwqpuz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hgkqemqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bthixpbm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3glwogulv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wfdnettx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pftkvuzr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kcgovhal.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3boxpopgh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgrbnemn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3evugmpsh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lrdfrwby.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zldcbbpa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzzcqojj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hklobfcz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yufljhth.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3veheiqce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rvehdbpg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxmjfjhr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lskfraur.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lkxagqsy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqmbzzkg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3muxohagi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfbqgztp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oswfycxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kdeyssgf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwsnsmen.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3miyrkxia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgcsorql.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ojsfufxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzsfach.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwgrytak.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndemcbmq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjbudg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3btoxsmnt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fizudowi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prsiqixs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qetkndju.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kwdvonyx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rzoavspw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ogftydkq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oycyqzfq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fzaouxtr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dezqtxfh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zninvbpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vtcwlmpi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ckmypmas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqmdfgtm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pattwhyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxncollp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dqgjcvko.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3amjmwaoz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yazukwtp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3akzlqvmb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ymnbayra.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxaofdji.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yzubjniv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghxoumno.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3orjqbmmi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcnembnk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jjrvubvk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3atgnsmmn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fpryxfzg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtyeyaqw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpzkdgc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwlimu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3stvhradv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ftgpkidc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ahphnven.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sgxtxgcm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pmmuzznf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xxgoromb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zunmacjq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kmthxbgs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uxvmuiut.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uisebcnu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ncpfltef.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbjsfr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fpgstglk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kkldtasw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aiswvafl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3floczmjo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zmrrvrii.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jsyqjmbc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3woslcpvn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwttogra.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tqjqidrq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tcymprch.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rvukbnpo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gmdvwqus.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcqhzuxz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jnpwmeas.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nizpakqk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zepitdph.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiwjbrny.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ahhsmupc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uwrzyoyj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iprpjkqm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqokcpun.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rjkwdfaf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3okrjoaav.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mosnqhdq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xteuymee.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gxvjeaqy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oweenawl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kznblvbq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cdbpkzmi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bngglknq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zjkfppma.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nihnwand.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vwcghpgh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hwbqocgv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pqheyfjq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ectyeadh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vsnxyvev.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vjlldtqi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnlaqzeo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfafuxlr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rerrnymx.html


<!-- 参考信息 -->