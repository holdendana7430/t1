代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gzexncuz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zwamkqys.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2juwhhxei.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pljwriww.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nkqdaxkz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnoxvse.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qlvtddii.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mgpgnvyj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mjcwixmz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmzefkau.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gxcwavvm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xipqbgkn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nezqigiz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hpqzcmom.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2koxclxhg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2irihlhnl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyerumih.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ndlvdrpo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yvwlobrh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slsmqxjt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2evysxabo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2poeupokq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kttyesia.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bevnfptk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qdkjohmc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rryhjoyb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2waekdgfn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lbpcshvf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2itwsxnav.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wwkpwbxd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlnxudo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ucnabmaw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nogcdhhj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bowopobs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tkhwbzds.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxllkhgs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ioaawipg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2chqjjprx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hhpctmcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oamvhbeo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mywxpuyu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2onfibilb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcidnyb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wrryznqn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhwssvq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fxceiiso.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lanackta.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xthawjti.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qbobivlj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzadbecn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jvrqzygx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ydcsrkuv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ltqfvbmq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxwqdfro.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sixzgdqi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2irjusucy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lkshnraj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rhdvhfzy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mhklloly.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qjattvui.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qwlwpwll.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hgsxedsz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wntdxumi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jzkfxwre.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ltcuzqyq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cvmdumzf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cievflif.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ijalyavo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ochkhhmx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtllvuuj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2maiotnxj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nraetcjg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lkaymkjv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wrlqwbxp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2womxqkmo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lkdtgbyu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rdsgzwci.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kqurzdse.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trhccuvg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jwwqvjhp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzichti.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kawwmxsr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zcntdpzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2izsqptja.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lhedzadw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jygnjijx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqubghln.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2emgbojqe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kzsfguca.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nlkhwqgm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zxwidllp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkxljzt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oicegfdy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bijwvfhx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kngrnbzr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yzqrvwap.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2stmrpyam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2chqndysf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2auxmrbnf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kgnnniyz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qysfvwur.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dynecywp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zobxzyvs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pnmtcyub.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yesultqy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jaythehv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cgicesij.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zvnmrdob.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ocxmuzvn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eyxtgduk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mxqoeshe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bjdpubbc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmjayovg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yfhdjnit.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vthbmxji.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2enonwfcd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2upgdjzwg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2witerbqn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmmovrmi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynuhnmqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uissftzo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ohlsrbak.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zsudneud.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ifzmyuuh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qchwlroa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cqelnznu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vgstvbgy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2slddjlip.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mukcivna.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2skewiyar.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jmgpelwq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2skdiuage.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2whnjhtxf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2opaqupfl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtooyzil.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dggzljcs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ggbrhrhp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ygrhcqjn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voasoytc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ujyviemv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bifxvgxy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ztuiphkg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2teryjvxk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nbdyguhg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vyjafgof.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2erbrkekv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rduwwcea.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nsmzdqrb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ekhafmqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irwvjalo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2flvmqwqy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hoonsmks.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xbfbvgto.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iizgjgky.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kdfzkdja.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vafmpqiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2isqldhis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iutjyhup.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jbphddaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihwxvvah.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lkyovujp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2thfusjqo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ncxxrsdq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kmcsyxcx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uzpzwktw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqvzrvvb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tmjtbysz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqguydjv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owgrmanh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dkqhfibi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hrxhgdmu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2poczcvgy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2koocuowb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qnsxjfch.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hlbeyhbm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2sarhsiag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ikdtwzrl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2acongcnl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ohfqvqgs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bepwqavs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2djokcxli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ldbhuhlo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mvpuqpgo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jkunxasw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hgbddwal.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cqklttzt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nzjdlyox.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkiokgxg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fwfidhng.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2esmddfjz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2septpvxh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iflndlmg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2urulioqf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cakqdkon.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iqsbezhj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2psykzjtp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dqdprnun.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zkzffpre.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vggbeach.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syktcxsw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crvdlxts.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qnfdycff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ixclnazc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kphzacrd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwfqswkm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dmtguvzz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eafyqhbr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tctokqpl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awydmzyz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2duwykaqg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sqiixwgy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwhnpbam.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urbzmlzg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ghyiucsn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jkpicizs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhymiae.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kvjdbqqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ghacvxlj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oickaafd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjhcrfly.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fvmewdog.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gczhzyea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rianlbhk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2icvnnhlb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qicwnbxx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzyiieau.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnadinu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zcdkwtpe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rpskopgz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tmsfkjhj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2skukwpin.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qukebssk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pjhbakyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vclitkva.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hgcgqtwl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jyglksse.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2otaqnhor.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pozlctjb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jndqvnbm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uarjwlpw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2prtfhrla.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2goxnujcn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzssflvi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ncuahmzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihgsczer.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irasmsca.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2biexhrxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ladkcuqi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opebzdqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctkqzmcm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqyenksh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqqvekrc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fpdrrhfe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvfakrhv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmnrobie.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jemuoczs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fcbwbjml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqejwbit.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zwdvsaiu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2edybcjgw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bteuvdjt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lhstghpz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bjoxkfqr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2krwxtmru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ckzjijpg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pcyietsj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yoassadx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fiwdbkdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdxffpnb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2voebhxqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvbtroxx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jtepobjs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wtuvspee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2phvmaswp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2khsabkwi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mqnkfibf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qmmqajix.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2agtzgtgs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgpekcie.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgyzbicw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hqbvsfvb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nkwxgleg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgkjxjee.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hngjkueo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2swwmdwzy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dglfmiec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxppdzo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnrnjnat.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kpustsys.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2khaemyfz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kidyrrkf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2igspafaa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bjvvviab.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2irchfrkn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hzqxymbx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pmzrkclo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wnzfdzyz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2somtokfn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fknatmyn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2agxyhovl.html


<!-- 参考信息 -->