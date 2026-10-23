代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ahjnwtav.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3sxybjsvk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gsakqkro.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qoaxsbqc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grcoomjz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smycnxjo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfzvgjud.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sudorjtn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cghdjilw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xfxmdjuv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hkrlcrgs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nxegxzgy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lggrmeqz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cabrmbdg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ijhmbndf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sprqhagw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tniagnre.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxqwssd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ilavivlh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hbbepeed.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsmhrya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3znvwfngj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxqyrax.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpljuhkw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3twmoaehc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vrxnepkq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3umfssevw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwsqaswz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kzpowjeg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mgcykxbw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sqekbxgi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rsftnfmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yijvxnkb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rhcxpcva.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zhqkzagj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qneooctb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dxbugata.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gfnjdkff.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzfzxcy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbiayeuv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhtqbjc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zjtogqtn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rxcusflf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3stxvgtfg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbtgxnah.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3yfqyeewx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jihmxrce.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvolaahw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvtvmjq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ilfpyldg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3emqwbvlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3baovnviu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bsfowota.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ggnyawgu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nvrqarde.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3feqajahq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fptkxztl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpxkrww.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjagyvr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iytvhvro.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3phyotixk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3imekgoyp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zucmofol.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3yplormfd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cmsjkeel.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3eqztchql.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kfasofnf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yqigyiiy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3atbwtnpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bbteeaue.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cxruwngi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ohmgsfjc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fitiwvzt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lqlcmmuh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3azbdyymu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kykxbpoo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnagzii.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wpfwcjwh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3khfouypb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fzlxfael.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3auhphtql.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rwmkldau.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gjkamtvl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ajhwsxig.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mnizsqxu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kswetrsn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3paravcsr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rdcufpqn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhezjmkg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sejmuaug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3obdhpzrq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jqkvpome.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lnabbpxt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lpyrvmmf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ovdnrbvw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sebslkyu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3groqdaeo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3katnkmpp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zkzejbpe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vupjjqbi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbjnpczg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfsupvho.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uhromqnt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lpwcnkuv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dihlmrrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qzfshtqm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rdteaykl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nmnebjin.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ddqpmbli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmlrhmnd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3chxgxxek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnchnesw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzctlzoz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rbpehplg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wesczfym.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zrhqzjju.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3owbrtrji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dflghfgo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qzbvezzb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tppqafme.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkgypdga.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hyuoagym.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3plxjfknx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ljlbrdrf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oweipugi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3inkvmpfv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3shpdidzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pcjbzmjy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3juqcdnvu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wvvjtonc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zvrxtzmv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wsteocbx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3khsecpnm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mlqvrpyg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvtcxww.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3elhgubun.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tbqtponu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kmjfgfaf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3khjmbfvo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmykgikx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ncqtepbm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3txwixmcz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3apjcegue.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3quxjwvzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jrspisfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cjfygjta.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivhbwfjk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wwjpnbfl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wiinamyp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yvvwzkhh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znqqrwhc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tczskqsk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3suuwusuk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3isphtrwq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3voqoqzho.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vekjfyps.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lceseqil.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ynvxljzn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qulnvjin.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rlvzqhgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgparcxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpritdur.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tdzlpser.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhmcyglm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icuirsps.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idpvdwed.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dghjiryi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nehuwffy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gpmpiapj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qkntarhr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qdtilohr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dzsltnxt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nsvzpyfi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gmqvnkbr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wtlvlsoe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rrhdasou.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lmabqair.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qufnrvba.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qjuujytu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wurcndhi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3spdnwsxt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3upveenqr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uiysgbvg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uvcezlrs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sbeensza.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wichppwo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3anzrtapa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nbvxnycg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sipjoylj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tfusqjdj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dafmmfqi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbuptlnn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cdkukmvk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hvqrfxch.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhhirqce.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihnermjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hfbnknmi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snlfvytx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ydreixxb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pffajoel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzjluwpc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwxnwzjw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wricdfty.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ceqpuzuq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybbhyour.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzonmrev.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3btwdnyau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wqtibpgd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rsjezvbc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flwqcfvn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gieddmhu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wrosaevv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gmcximnt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fyetzfmq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fmxciach.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mqvynvnv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xtyscnym.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ybfzfejv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zrmfwcen.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zmcpzqkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajcttrvl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yhcqtbxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqgerahb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xixptpiq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dpiiunez.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iggzwskh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lcprebcm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3endzmycl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jnzkiloq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3givoalcg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ksqfwobv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jricxnxy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3swnzscii.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ufwsjuvc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrrsti.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjifxdqo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gygvgeys.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvhxebtl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ukwtcuwj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddlmrzzc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czncmtwy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gfxrgqnt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dqhfmcva.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3flfvxsyr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ukylzixq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3secychmn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3apvwjggk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wdhxfori.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fgmclktq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ntswveni.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3umvjaxky.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ppvofrdi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipeecrzs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvbobydo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkwclyej.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekevowmt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tiydvlzo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3coemhoss.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3djjmjmww.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xjvvjoud.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yxmzoteu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bcdltrnq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3inbsxfst.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oaomcvui.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzhybhhr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fcmvntqs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmwvaibl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahdwlezb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eqjpzsey.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hlxnhsbt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzoxqfqm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rdjnzesx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ymxftfwf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bfalncid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lntparvz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ymdemfbf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xflttzqa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3djulnfnp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rmmzfidc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3velsveda.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fpnptpqj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zvdfdpol.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3omipfcsc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3umipxxqc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uqsaatyc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3igqempsf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xyrtddde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rgmzfwel.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwstjikc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqpicyzs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mvvpukjh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3afqvgapx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ihmyubty.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3icjaeyal.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mdhuzukv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xqpoyxdi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xsowxjrn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfnarxkp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hqpnoazg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwjclfhx.html


<!-- 参考信息 -->