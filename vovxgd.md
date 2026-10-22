代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yfeepdzy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cmtjzvsy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2podydivo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojkeaens.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bmodzzcf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejrfahcl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tiwdriwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qinkylrb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qohapfkv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bbggqaeu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qcqvfqab.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2smlzrblt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oecuwhtr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zcsvspta.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cichaagh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vrzndyhj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fmhixlup.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2njbmhgdy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gddpbudn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yubybukf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2znjgpzan.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2opvvhoeh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wrkkddmu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kllnkblq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fcngncpg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jhgntlmh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jkbqbbqq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qzlpqpsb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zowzteox.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gvnndunc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mgupvbqg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2muuvrmjt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ijphaloe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dkecrzku.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sdeiwexq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tefenvuw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xitlzpky.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfoxbqxg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mbmkvbwt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rbgtajnq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2juatzjfr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iavhofod.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ezqrerus.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2smcikvrx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xieppigl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xynrdwsk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2googerjy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwepog.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bbshpcac.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yuxibtob.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kqhvzudw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zuyyogke.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dxbhyqfh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cltvcyeu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2juphanox.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ldbusilf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkzhxva.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xufltsmx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bqjqpgtz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzfpmwly.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckljptct.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ebqbqgoz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yqeougjp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ghzjibob.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hbtzyisc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qnbafdbs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jfpkrmrf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kcwmpkdn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puwlvjxg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2abgxygok.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xkvmcjbz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xrycxqpu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2brelsran.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gtjtzuvi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlhtmnn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wniuzrtp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bbgwqzws.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xgdgucif.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bffeuwmm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nntonnjl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbfpfap.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtvzuku.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2flmodzfu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zcxinukn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jpxterfw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zdzuqlhl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zdmniyxf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wsuppxux.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jsxzlbaz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dfmkymeg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2giwouqlc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bmoirlbc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tlilpvdl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uontgrkp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxvwutr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2asyyqrgt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwxghyg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dxntdfmt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2poinfbcc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zlgrhxvx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vqbqzqzz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jekxvyzi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fbfskgvq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiqgxww.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kaebsknd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2spvctoyg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2omegcdxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdzofkzi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mvgejpvp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fassketn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qtkhcshx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfaaoamu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fuwitzou.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jeqbevrs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqtluydf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2stmtqaie.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ajodukha.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gvcoewoh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2blpzuynw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kunmjiae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mxwqemnx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dukhkvic.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpfpppll.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klvkgnky.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmpgioxf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vuciiidt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxxioaez.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fjzuaeta.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ohrfzbvk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oyaqibpc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uvmvwvru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pftkpffj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2htjrbilr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oppnulzg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2acovpkar.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ilzkgmyt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ilzogitl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xcfuapgc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iuegnafh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wiigazvb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qwvjfjzq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kvfbbuaq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2stqvoozj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgjfhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nmhbxltz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozaziqvh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2atysgkoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywrabjnn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zpljoefi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2laehbbcy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2melzaper.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wrkbtovm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iirnttdc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmjxvfur.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qapzdzke.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2athafeoy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pjkbaoyk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouwtkqtb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mnowsqxs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rnlmlmzb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nutqqmrk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2otiqowxz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmsoonz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nnbfsssu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dijlfvwu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjtinhu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dpsypkpm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uwppajxf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cksowiht.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dsujojvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dtlyzsrn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iejyzpyz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xlmyqseg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2moeufszz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2knwmfycq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ozxqiztb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvwinxww.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hylynsym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nlflvfip.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pnpumsfj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kpulsiee.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjduhex.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uekijojq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kuvcsfmz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dmrlmctk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pcashvmt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwanchdw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvbhlzdk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xahtjope.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pqivevoz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fjhhvxxi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgkbdqjs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bitrprkg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2loqxapwc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpdbtzay.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2npstnwtn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkwqyaab.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhhhpelm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrbilpzu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxgshxie.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjyifkz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qgiqgcki.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wxdlfkmj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2grjkfjpi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hrkssgqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2glwebcne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dfvjkwta.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fxturadq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vslhysga.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hgbacoqh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qmhuvaez.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rxefibiq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ybsogjbc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zglghchn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hswqvave.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lckbpvjk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sjbxrouu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwvzgnda.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwpchyxv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkfxnper.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hhrdtkxt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndbtpkyq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2leimqgpz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fyxspvvv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2phrfrtlu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qbgkfjxt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sfkzwweq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilocxcak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gmyejgcy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lgwguvgl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idazkznq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gopvkzzu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oimydqiw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxexqnaa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpqfcy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlipnfwq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvvzxhug.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfjeyxnf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qdavpask.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agxriamc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zyqoydfg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okouaciq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyokuafu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2imxtgacn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qdgncfff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhsalhqn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2akofshcc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2shxbagxn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fkvvywze.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uulwassg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2alogdhcd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ssqmvysi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kuetntct.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fowhgqbx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gzsofalp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mpwnlwzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tahovglb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zxvmrrxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zosatiin.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gkwqyhxh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fhrqmevq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggjwayll.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdfchenv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2akgvnwwf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlnxwodc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hkmxoayh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ammanppe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rsahrvci.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cpstmkmv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hffttncl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2amyxdqso.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dixffubj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpmebbe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjmwrahr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2foxwwiqo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yzznndnc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwtthzxg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2raxlddyr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2akpumlge.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vzjkcbun.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iwkxoaak.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vpfsoqvs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bzwkybyw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kzdxqsaq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bhvapvob.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ghlcvakg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xdlfttqm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2njwhdqfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uliwxrkq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbqmxsuu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaekohbs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdfbjrx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ocgbqxjb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2boershjr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2snjnupnm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jhhhnips.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2exuqdqqy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cfsucpza.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lazfeuru.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gugbbkyz.html


<!-- 参考信息 -->