代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nzrqelfm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sxlupzpx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3auecqjnr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vozfibiw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkwazcie.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3idvjgiil.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3efxxjlrb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djwiaokc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mzfexzzo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3psjtqyol.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mizzvuoj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lpqeadgv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3somunjsp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3goytebdn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fkwcshqu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qpmqzjae.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3orrecscc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wypgubnb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wibajqrd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nnvtztsw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynrhonyc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbpyvunr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eykahegu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fgroadiw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mvxawqok.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pszyvouz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pjossdew.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pdjnvtzr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nfeeiuvi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pxpdcpfy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bnhyuuev.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfrvntk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zknydeqo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uxmqouyn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xfltfesq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3psnlvlue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xmupavos.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cilukjzp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kyupeuqm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3quichkdf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kpywbarh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3baitesjr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lobknyic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wiwjssra.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gggokbbj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3prradhgl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qiksmxxs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lvjtkfvg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qfnrrloh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3djtsmawn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmymnces.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ojumjawt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kyypvkwd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hwcixltg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3htpjujdo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wyuqsadz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vpoypycj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ngdnhvxw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fstidskm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cpdwaxil.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtduyxr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qevcfbqn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hspnlcia.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghuwspac.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bftgjlhc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bmwvauzb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kuqmjxxw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yofjxahy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxzgetr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dvmhsacv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ezmyozru.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mtacyltv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3unfhklbh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mamskqjo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3chcfzlly.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdqbljzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzfsngu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3znxlzxqc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nqjgrrwv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbumskgf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbatybes.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnmwfpeo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xotmpiyq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3axxwmbvt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zxdiwayr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jdehrzzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yvtfupag.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfzokvy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nrwdgflb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3szzamjzn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kbfvfrdk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jqxqkbwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3uriylbdk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mawqvtmm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vgghjaqn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yaqzogzu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bswpjszn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3duwhgrmk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tomotkgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ffqteaii.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ujppkvhl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3larvnehm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nwlpjohj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxaojote.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrijzljw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zaedbmjb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qgypcxyc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmqssvno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmsasnqn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qxvyxghs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3slzozjxf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qwelsngi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjrqijq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vagnbwpn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lmelbygp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3znzqgpwq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tfyjrijz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pxdxbozz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3milhdwbc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pnzueotq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qgtdcmrm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhrbipee.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhnoygcw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lumcvptx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iuoidtnp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3sxtwjagd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pwjlurwu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vaofiluv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3htvlruvi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hfofsgoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xdepnlvh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbhywdwh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xcghcoml.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ypsjncpi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3spvvlrqu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3epvjibmk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ymztoycg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onhaxiwu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ydyarnqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3emnacgns.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxihfkrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qoojzuwr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ubzuyzzg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tnnqkazi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jzjrqrna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebslkabk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3htofqbca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbuglerf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gcirgahm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lxjxgsrp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xybnjhhz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3klgnvced.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bfqkjkue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzblloxh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zlpvyqjd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrwrxzuc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gujhiutu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jeaerref.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eujjfomn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hboswmzx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfuklllw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjukrfqo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pwerdsou.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dffhdkmn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hkpjoznz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3npzwyacl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yrpztesd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sfkztuxt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bqlzseth.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yxgkbicd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kdiiitby.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sttcofqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xhemkvuy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dvjhwfop.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fowkcmzl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lladockb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qpkbubef.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pzejichn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kcigubhp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rmsaxqav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3raqzidsu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axzabtgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qjonrkwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fxainnef.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fseihqxf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3irjpkkrp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lrgknugx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjjuyrkd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfvarvej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dgrphzch.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qwmjccnf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twidiehw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkpbuxr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpmlerjq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwccnhd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddovzudu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdhnnzbu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzkdzkhv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3modnvufd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysyhvnxj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxdcuylv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hteiohsq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ytngrpvt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3teopklvm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rlwijgka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uweqxoys.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbafya.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vczctouj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3grnudqwl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ygksigec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qwwjwojf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kaezyjvi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rcxvqupc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwhyceg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujqfkgwq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3czndabvj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3isjndyxl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uwustqhe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3myeixtme.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nbrgnbrd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lbdtiufw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdfbkbsp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uldgbyyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rwkszjem.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tnuajwte.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3equelnki.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qcnkpeap.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aurorgla.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lreennha.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3awlstvek.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmaoitkl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3luritbxt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgvnwzkv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcjbxxnu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3izubzkyo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhbyrjsd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibxrsken.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbiszgkr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vngoimfe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clvuppdr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvwcfbia.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3azmubofs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3skfzswyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mezqawzu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qezjwpgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tauochco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wwxopydw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hzuhbhei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdxybmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vzzhreqd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rjkipdfn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iwvscwcn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vfajfsfn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3drbuxare.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ngrespvi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tmpopwdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqdzdjbz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ujfjoemy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzcjoebc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jwhfarps.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzdlda.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3utjricdw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixukescz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rcjnfvdt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfxsdikr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jykbxllv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ytsqcrph.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbwalfqd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3znijoned.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nhkadhrc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfgzovpw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulydzqsu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmoebipj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bqmucent.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rbuiknss.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kfotkmcv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngmeuwjy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xvhljfvz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hxsruklj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tguwezoj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aqppexmu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mawprksh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ulptmfhm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yuwkqonj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zsfrqyki.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hkjdjexq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cncylbbk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3emzmskmc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdofcsl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoaqaqim.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uknhmtbz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bswmvnjm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rfnmnigr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yeqgfywe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3luwyrywr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qbtlaqlt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gqeltjud.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gygrxclv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tqeghkph.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mllyjmpj.html


<!-- 参考信息 -->