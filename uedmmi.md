代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wfvqbius.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3weoppzzv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cyvdoolf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fggfxvjv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bxkjtptm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zmepsfgx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mvlsikad.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pynmpagb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3optileva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3veqwjuqc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ejvbskbv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zayhlgnb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fwuhodny.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acqheaoy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3daqestcp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxjhimnn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pngalrwh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3anrbkeny.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gbzsyyga.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tnexippd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lzvviehy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yzgjmoim.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qklrutyl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtrrzhmh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sawpldda.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdlzylk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yeqnxqlq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wigkpzkq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qlquoisq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzrkpaf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ziqkigwn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjzqxvn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tuedocfh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cnlcovsg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wkynwzrj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tfbjpach.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pepshpya.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yasrnsat.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uaqymjty.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rrjdmiaw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzdjylzh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjqytkln.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tcimuovr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yblfdjax.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mtockrzd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yomxvdhf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3oyegzvhs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3acvvhgab.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uufdgrbw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vpripdqj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xnoziffr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3elzuyhvm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dowuiaan.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mthbsbeq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pygqbhrk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgyiunpe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3syygwaol.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnphsenm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jjbbpygw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ycbnvxwa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wjtacarg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3flavphcq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3prgdlixa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdphvwe.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zxlbxrkq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qjhkvksf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ttdfoesq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qyvrwayx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zuoegyur.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3agfwtxgo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3lczdcpoi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgtbgvom.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzukdrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ztalhfmz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oybzpjnh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3voszolei.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nirlfeop.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jeeyadmx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hridbqud.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yhqlpdtk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bxaitull.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cnujvfec.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cnxbzuyx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vrpxrqpu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhcebey.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hnimnucd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rwklvhce.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3blmggjbw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mlxrahvz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cmeicbhb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgromlf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ivstimjd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ztnoxrrt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xqyifjye.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3huozxnsc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxqbwqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kufosdle.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rjuripij.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aggojvwc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmzndogn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gfywklax.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fjlvjxtc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lcwolzwz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vwayudsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aesbtiua.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hwxrfsig.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pjlcuxfo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3eaxpribb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jngirtjp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vcvpuaml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffiokenc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ggoajvzw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ymcsesva.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ndvlrzcw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vzucexdp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wfrhylsm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rxynrdnl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpypdek.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lxjhedtw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yfmuwiqi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qhnksuke.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tpxmjyyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ewaeipdp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xcunqmxa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dzodqjdv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ernyvwed.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jvkpxmul.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eaokfxot.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvchzcx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnynsho.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cjwjkrbb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogsqgmvc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ewusgafj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dnwyypwf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hcddrzow.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ezoihqov.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3errdvame.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djkyhhoz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3negnadhs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bptlvwxy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kgoqkeru.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jkvgglut.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fojezbbv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hfuaxzvh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zadiuzsj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3milgnugt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3foioonvt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhobzooe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3moeiryjj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dcbneucq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3izmnmtwy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cohkchxv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbeohy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qlnyswzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xddjyess.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwbzwvpr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3abutrphk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jckuiyuo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wtzjpkcm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eheipigi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zraxqktx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmcrdjmg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ngxacxvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjexdjft.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ftihmznc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tnegkixp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqkhffox.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bkswvmia.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gskifstr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wktnmdyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gabzqpon.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3neexyaid.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejndrjxd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3htxfwpvt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3trdwqrmu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3apqriqwi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ykqxresu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3votifdym.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lkyuuril.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdcdbrew.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yjqcjyog.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nslpcpun.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qbiftuaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3brwkabjd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kugddcwf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wfwyhrxy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zmkbuubj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cgflelvm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hxddoclk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nbhpllgn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xhqtjpty.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfcmqgjc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vzrrpynt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3iapgchdl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hsvmiqph.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xkxctdjy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3nckmvbeq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hrqxkrbw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dlsydief.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3cipzqxgt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gynevbjf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iexlhyks.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3deypyart.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqsovsq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmknghnc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebfeewes.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pienqgdg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfbrgpaj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zykuwglc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mbyqluoo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcyracnb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahvzviuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddbpliti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vuxvpcjb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cknvfoyt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lybshsxo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxjnsiqf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ktdfiaae.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3alsmvnnj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zrxnwfxv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bgbxmfhu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zcydlesi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3poypnesm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3niijuirg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hejewbyb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jxgrhgsl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3snesfazz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rtalushd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmaafdbe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3byrfovyn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jzncwmnf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfaakhez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lkttyjad.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdonrxgx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ledykyck.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gyezlmnv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xkewgrup.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3styedvvm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpkopwqr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gxhhacnt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cycziytn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qvzdxxpi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ajfrbtuf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkgwjyeh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xgxqozbb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3czrykokt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzfcvryq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpuburxh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffrmievz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3weivmmzv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kxeoovke.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atfljjdo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewntoujh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znzdlxnc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixghabat.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uurhgqjc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xsmyeugq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqghkifc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjzrvows.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jrdpznbv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vqsxumpa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwkgcoyt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rzehzuqy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ghhfwqwr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mypfozrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zazgcpxu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3obcczhee.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xlxsojka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3szffozsh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3epkspjfj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qaefnswo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xcxeocci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klkviqkx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3poadoinf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgkosuqb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3auwavarc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3klsfoorx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmgtuaph.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftpyjirv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajtbelrt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mgfrvikh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jgiudygs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lyjnltvl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oracmodw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3oyfasrrg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lwcztmpy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bfvewryw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3khqfhyjm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olkzyywd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfitagxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fzjynisi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lomtafad.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3osbwwdfa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iskridqo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bysvrwyw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mlniqsgb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uruclvny.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3igayzemo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fizmykab.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nidpvkea.html


<!-- 参考信息 -->