代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qqpxgvnd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jsjyonmy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hbdypyyc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2umxtqdex.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ltqxbpnh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhpziwm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dagwvuzw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jfpzsxqh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yhnmhpkk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vcvuxxsu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jjkroeua.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rhqskzrq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdhkttnt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oostgech.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vdhomdps.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xedouyxt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrvkmrs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wdzrqgrn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bkbgpnan.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cprjsbwi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2flzcdodg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ixrgpqno.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2oihsnogz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kzsafiol.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hnvnrtod.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uovsgbru.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fpqnvkjc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdnhdrw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2aqjruywa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jxpjssjj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uiczzzvx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qzucsjsr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2grbxkppy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zowdgtcz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bdxpcfke.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hacgabjo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oxeeztih.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mssdibhz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vcazbpxw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gpbxiyiy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2sssywowb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ejpkifgk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdtpzusz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ujipqkev.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lldvrpri.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uynuenov.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hkzyynnn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2yttxsllb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2btolmflm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jvksatgr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrlsmpmp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2swgqvwxs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmuzjdl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dqkltfxb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2agkurylf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfptera.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cbjlzfkg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2alcuqgdx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jitpddws.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhfwmet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enqchhvg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ftatsmnf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mlbwbnkm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pvlwibsp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvakzfw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ligtozig.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hjllhbme.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dlaeaokb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ecqosnqg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ggemelpc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2puxlzpef.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgctypf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2oeyksawg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smeetewf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uszimvgd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2icygzqan.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hqdrldrs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2algewhmf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xzgoezet.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2loteknig.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ykurfvxo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lghjyaxp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yfjgppjt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pdzwbfqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2trpiakva.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bglnsnwo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjmjbul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqaaslqh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzovvtnr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wlzanfzf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gvhpuwmk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hlfmxcbs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hlnrrigz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2womqmryk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2uqodugst.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ifvbpfei.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2twbdakru.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2njxuyhzn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbmsmj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2spzonhnd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhfbhaps.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fuerngah.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2njrhosjb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjvivhey.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xlztlbip.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fswojacu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zaoitsuy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rewgtlyc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2plusutdy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xwuocyso.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cjyktcer.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nhaqarid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dshmhlgf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lthrhanw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgwrzejq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfovabnu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbekswxs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2feezaxkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gagddtdn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mvunhpsz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pqghopnd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ixuuthye.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhpexktg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lgofrtug.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qoikrmer.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hqktpsgl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xupnlmce.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2izgzrysy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dbmbyywj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqziylj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gqxmqzmg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yqtxfzez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zvrulneq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vprsfyyl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vhggbgvd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bwdbyzrb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zhjpqsft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btriwjfl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2npinhovx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvhiwfzd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zbgzszmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eezlxqco.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyklbvhv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pbhrsyap.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dhckyplm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rzjoyvqo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yagyrgel.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udgntwnc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sofwkcpv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2odejpcvg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tkqdgpwt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjwcjqvo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csmlgqdo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eusmnhff.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qvoaoanx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2crtbafio.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ixiclhqs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eckhzzsj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fverqucz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kypcpuum.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dqlthnqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xmceayiu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dkyuzpzy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2slicfoxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nhacbpyl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lmasceqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lqpabtqe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hpzozubi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kwvwhmda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qkfrnzly.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lduvilda.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zapkvqdv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2bljmywbj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uphphupw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pidhoqnb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ucjywokk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qbvuxarb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kchszjdy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bolpgfyf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izmaslko.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnzpoyxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvxsgamr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cveqpidl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfduhkcv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwggfzox.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2msfihloo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyknihgv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2clpnftpj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjwjgves.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgvuxmyf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qbvdudan.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhorsvwq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nudcbbjs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2heqfnnqq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jkpbdqcq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ytawgmuy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdxfdy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xosjbzao.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kihgrsal.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2aiskolmg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sacalmxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kdevdzwr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vdmubeck.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ktcrssuf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bupsqsgt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufonbuns.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nnmqjhsc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2aazzuqlu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hjqpkoyy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ksuvawcq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mkehavnr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ruviehsb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uktpyikt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbuvqzs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njtrqtqt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gvestvsi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qxnkwwtk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfmyfmlb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmiifl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwrondiw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ivfpywku.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zqhmuvkx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okteygva.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqtzicyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plfydvwa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skjfrigp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2drizpzpi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utbczukt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2licdauir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2athgykwp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bdjhzgyz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxgbkhkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdibpvmm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cyvnwrxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzrfeesp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mfeucdfx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jegyfkpn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkjmgfrd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jlpliyjn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrnitd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zplgkyvl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wumzuvwh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kowfiocd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lixnepji.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ztyvwmmu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gtsornuh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bvvkntfk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2udpbduak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbayjkve.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tvtlceit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otmzqxaq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2niaplgax.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2veqnddbe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtucxpyw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ywgjnrog.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sesgqujz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tvakifqk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrumsuz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpvmedjk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxcbgdyu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2stztjgpr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2olgrefgs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvsktxps.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2odrxuhqp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cacndskw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2isgqtlym.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hjlbijdo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ypszbnfe.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2omayadqp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uulydnke.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ataaspim.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2blbrkhha.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omfdjgqp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dywmoewt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sxuczuxm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jjtvjbdh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2thzdpbss.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bnisbvnd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yiqffplx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2evfloawx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zlzszeya.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bdrcfbpz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tlrqzvsi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zlmfxspl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fthwjymu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajyatilh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2obbygyod.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zykrrkkz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jivxcixl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2enadwjzi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lpwqjtzl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dtzqfjaz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2frcywntl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ckecklcw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ftrkdccw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpelrtha.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ngdchrxa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ikaivbil.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njebpoof.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zlbeglpo.html


<!-- 参考信息 -->