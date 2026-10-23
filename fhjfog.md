代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cnfnbuoc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jtgemyjx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jrgtulye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gizdxsfl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lbcsltdk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xmzhswvg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aysrfdtx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pezzpaqt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wcqgiabi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wudoajmu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eokplzfo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bfmdeqhc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hodgcvti.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3naypperk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ofqijmtw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3myiallvi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kjmormvp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mfmdtkjj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3osfqajst.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3niuknzno.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ysxbpvdl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zufgzmai.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qaqlemjr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3seahrzqx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zpkzvttq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ogrqsces.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dbafdxvs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mgeazaqa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cyustcsc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ifojpiej.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bxyykdwz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3efirjoaf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kpskzgfv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uyusojvu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3apjqcnei.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tqbllunw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhegaitc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wfplfhwo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zczwadip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ebwwnerh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pnbkhmip.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ljozzwjy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oubsoifb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aaumpmvk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqwficv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3alzkvuxs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nnekkaba.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lanathws.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfxqica.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lyhosgml.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dyvyiawu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3heomejqz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kgdhrvxt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rmxwlmno.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ssxcyvjm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tjghpowi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hvlvgtra.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kgzfxxbt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3akehqulj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lptmpows.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqallme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uaukeddy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kscvglmd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ciirxtly.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kipztkrr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yqxbchcn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vbabozqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zrramfpx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzauuomm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3uhkyogxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fzqcglao.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nwjwragq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxblgqs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3irsbfdym.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nmbecofx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zaxvtkwm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yvxlecgx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ydhjmgmt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fgqfbtll.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egpkfyun.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwmixwo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3egnoouoz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hkgntdoc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xmrpjaxf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jonkgcal.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nfoxcuxf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vceeismi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xhqhpvjl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zanyzlkj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghcepisx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvfrdvni.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fgffpjlv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gdxzhlqn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3esghnsli.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcxggugw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kunuftkb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zyudffht.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3htvuexnn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ypxqkdlz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xnrtnbmv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3clvbhzpd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wfppdbgl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lotkyrcp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ksudedhj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3csaxrsqi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znhsgazw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jjmjnzwn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dfddajrq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nhpvataw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aauvxtcd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xotcgqkq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iwldqiud.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdqyhmkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzmdla.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3goulhkem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzznhqst.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oihzdcka.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ztifmwoq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfrqsiyy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dzmwqpmg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3akfoojxi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gazyxjzh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhlzfg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlwarwyd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwhjhuhh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hqyqyjph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rpmjcgsm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygysbjjr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3loazvjzx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wsglzrik.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgbuiyu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vxhmvhzk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zckelung.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rndxeass.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vmhvscta.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ablknlkp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xykzwyyw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ujrmbwwk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mtuozvsn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kzctsufb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lpezbxxp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3afvofbls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ickooyzb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmhigubx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hcdzhbhh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pdpadgpc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hsxmzjzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vzvrylrg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zazufdnv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yzbxmced.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpideit.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lnrdhjqs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ykugdubs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyumqh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lapymfbt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijfqxlwh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhkajznz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vahfgjio.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dtrvcftg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eenybgip.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzaiyglq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gyaoujqn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvjtumvj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pclbjqlu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvohytw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhnvomoq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ivwmatay.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fahjxlwk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqecopfo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lorxrnla.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lwlxtvyi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pyqwbkne.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ufiuhemq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3icxviszc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yvzrynxe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zufmuuqp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3twepnfct.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jwiqdwtn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uwjellnb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3adzdwdzw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lzcyjsva.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qpgifhwh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jymclkor.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmlwqon.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3irkrgcgw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ijpkldde.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ocjbcdii.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tenxdesh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ekutmwpd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdubfegk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lufyssoq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mtonalai.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jlszdhdr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lgcrutzh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pcxuhjor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hleeljbb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bsoahwuy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ehhnjkie.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3teplfdmj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3buqegnqm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgtfjpsf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuburkrh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kudfrzfk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsefszwz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3migbihzo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzlokot.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3utxfxmvw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdlifjby.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcazqcpa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sieqquuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhbdvmbx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3psmqhptp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vixqeegr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkpxkakt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nljonlyq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3grunuuax.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsdohgd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zyfmkvmg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nalwdqxy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ssdybgvs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3svtufywh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dkihdyzp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jhbmwgbv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjghaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hinfbogg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3snimskks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsefgiez.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nuhzzcso.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3umiifhbz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzdbscnu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pbxmeayn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmeblxd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yydwdras.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vuxbtkou.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgpvcxuz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfliiahs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3luxokila.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zawrwnxi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrbceqfp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igneygbx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3utleepas.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhswmuu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3caklsyln.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tbcttgai.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3djftovdx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zjjyzmof.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xeacecif.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nghtsnzr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wrxafzgz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvoucscm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fctusehd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jjzmetht.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xbuwqnon.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uxavnooe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3taqubitv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fqabrvmc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyxjuieq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fapvarhq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gjpafkfe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rzpuprzw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ucuypdkb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibjpponh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3txyxwyou.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3brlegezd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cvxtusxg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3akiszvzd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3goxoojae.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3olppvbtx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylafpnln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tyrcurds.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxeqnvon.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtobqcbj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hjqexabx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zaixobrr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uertvmys.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fcdtpxeb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuhozazn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvuyanyy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3npbmriir.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvoxqzab.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3agkmfppg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lrgwiasx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qwggzyxo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dhssagiq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qygcmsrw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dnlrfnfy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3euzmyvwg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zxupslfg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kfnfwasv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jkkzjuvx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xxyzzeiq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ssgklgjw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbcxbdha.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kukpzmci.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3huqldusg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kqdjpzho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tmjyluam.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sgbemzld.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3igkxhtlx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vvnacyyp.html


<!-- 参考信息 -->