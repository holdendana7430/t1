代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlzdctfc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vmwhxsbj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rnasaxgg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hxbcqejn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mtbycgkf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zwepngav.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lebzmubx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rzuzffmx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mbwcjndm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kjwetxji.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkoazpku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yeoupawb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmggvzyx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kndwwixa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmgzufxe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zsejbugx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwdmucu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2roqurmik.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xbuofdrp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2muiqrirt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kxwwieax.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mlvdokcu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ikfysefx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2absoyveo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kqtigelp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtqzrmo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rgbvyzrc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mpzlgfad.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gtozmstl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvmmpbnx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgemqsws.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hairyczt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dnhxypmk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cnrhhabc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwnwink.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cfwiyqks.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uarummxg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eajdpoua.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zdfntmff.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2amcjqhbz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2likasxum.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2witvmkod.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wpmxsgsf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hwwzrclh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2meplgzsg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ffvhcmgb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mngthiih.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xhvbiwur.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bfbvsqga.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxduxhf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nnbsmjfi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fjugodfg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2isuolpbn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bwoacybu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2psgwrqau.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihxknmsc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sypfrawd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyvewhie.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yjosnopt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2azgntiyd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jfthybqi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vqgbqect.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fdnkphjt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrelnrq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vfamsgmh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2crzxdend.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kvogrbmv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wmjynexu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vgpnaltd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qsgcvthb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2uwoucbcp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aijgjrje.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsozlfj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wahlujca.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dzhcwzyv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwqsajl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2trfizymz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bmsoivml.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vlhhnmye.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2osxgqzaf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pqyomqsa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zhgxtwmt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uoqkkeqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ojuqefnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ehezfhld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eqebimog.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2unmdbjjp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ugdxehzs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ceocdgot.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fodsiqmo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxightr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2awxvoypp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbydzqmf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kixmapfu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sjrbcvvg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xctktiyd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsrpzlty.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ylobcmcz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nlmsbmcn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rldrnccf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rnydhlfd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nbeujoah.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2enekqkzf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmahdyl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kctjvddj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvdquynv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bjyjbjqv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aqgokfxi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sisfewtw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wuvaxaul.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qmphpzxf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pqkhedeq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfinjylx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ostuagzg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fwgsxinw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hgefdmkn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wsxzhugx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qeownxij.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2btzmzkih.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mwgyrroa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jmkwkmys.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yfebcsae.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2artbcgco.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mufayusa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2roxjngqt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dkakmojc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gfhbcupb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjayryfp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfovfbip.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nvkfkeuu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iarmkqtm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dayoavqh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qkmqjdmp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mwxjrrej.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2eunqqndq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bzosrppq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vxxdqrax.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgnslktl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jynyxulm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhgvmvlr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxmjmxun.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ickagzxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pggpwsya.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ocumewdh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ygmmtqtd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxhjybgq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qcqwcter.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sobpmhes.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rmgaquvf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2istdqkyr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xrkaoyrf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qcjielps.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qhzrbqrl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ejhmalnt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sbcfmbss.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkqvlzme.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lteikzem.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tpopvtcj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bpclcdxk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vauklarb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xepzeuih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcfrslxa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uqufrbtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqsvmlfb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ywrjmaia.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wmwopzqk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmvmzzhu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2evvtpfso.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jfnhqlje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aftdxrkt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fffyvzgm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwrutw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2joqltwdd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xanlersi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cnuhizio.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mokdjwak.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhnefqad.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ltsqgufd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gtaebbij.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2epyxtdio.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fljgerua.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ybnuriys.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yhlbpcui.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mrtasgdh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2leorehrz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ytnqwrzm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kiwbpawe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rlirasfi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kwlbppbo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bmmclnce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ulnirxlw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmxexqhr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nihqnqeb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fvgpiszf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2votupmqb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pcnikcvb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fskigxfs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2piizlbsz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjwkiekc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2raalaxix.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lubjepdd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jgbrhhrs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oajmtekl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvrtnttd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpxmunq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2okrocgvo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wzvukjie.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbqiryh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zpyqraky.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhmteeum.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzvwgvec.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpspnvfg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbjtqwxc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osqiaiti.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qzhzuelg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmzlbkhs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewenlrtg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wgtdaqvk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vadefgvd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uxqcyfwh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjvryug.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hywbblpd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ilguizhm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2esaxiigb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2icobuazv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mobbhyal.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ogydkmfj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gsugzpkb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nqujlzli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgwbyop.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qgthbrfh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjwmsok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gdjrdzby.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qbxlwinn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nqpjknma.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lsbnjrqy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gugmeohh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhnaarif.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snekmrnn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cbhqniya.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2daohrinb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqaoiyal.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rlavjpfy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhayfnyl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jawuspql.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lxahaibn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smklhele.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijmqpxsm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqmhbyg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gndnotvh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wtdwvkty.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnzvyfvf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yitlypnm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dftwclir.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ohvkkdef.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2beqwkqgj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvwrgyki.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvkfmjsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsjrnrlb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ssylzefn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tbdxqcqq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2foxrfcbj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2baonvzjx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uiyjmntp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wpddlakr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2pogdsnad.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ijugnbza.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uwmgzozu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eyjyxebf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pakknjks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2trqezmyl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mdjthsvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqmmcbza.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nqkjnhee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cixvzvgb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xpjhqoyy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ibgapuwq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkbcmfzk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zppqxsss.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciirybhh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nezzsjfh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2smjmmkqo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2besrrvtf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dyhjjact.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sqkdngvw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2auyjyihe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmzyztwa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lhheqbmd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdmouuqu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzgpirck.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtkjlxs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuslonlb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fkfklnak.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cmyaprji.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hiusvlmm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bbinxrkm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oytsvqqc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tnloaawx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jdxssgkx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gpvgmyyq.html


<!-- 参考信息 -->