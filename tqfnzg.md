代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zzdshzkv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xsftbgsj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dxihripo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ushneuha.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zumxexje.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hxqpgfor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eqinxhow.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2byuifquy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bqnvgsop.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mwhyvwia.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2thdqirfh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lhbprsyp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ugriqzll.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kluzakay.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kurcsjak.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2itxbooql.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wkandzzj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cmpbkayn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cdolgzcy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2znsfvxiw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mfzaitzl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdsxgi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2aunoyezy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kstlqosv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vaqrfccg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aeyutcbm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2eogsonxs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hiyvympn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zfvzfcoo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kezxrexz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jckkbxwp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2knjuyhsk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rubowzqz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkyofux.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tebrpuat.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgzdpwi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gpjdlpwq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvnpxtuh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqtpczm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mlxqjcic.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2puhlxutc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ympirhpw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghshnquh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jyzegggb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xrbgwegc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rcbvvbxo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2skvoigsj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vhywrfhe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sbtjnnmf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jyvkxybm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tmtafjzx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pqmjnjpo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vbnghbzq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wlaxmual.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xkkpvrdw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qrtlagco.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2htdephne.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zazzsxri.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zfwqwlgb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tokjvilc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ryhphonn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yxtfkdqf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sbdekevh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mxfktxew.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hszajwvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sllhxhkk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cjgfklks.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hvizuokv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lvfsmdzz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cligdiht.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tkacgxgu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2skzkzaay.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvtorgu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvxlgct.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rnzwejxr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jcowifvh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qytuhavd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qidxonss.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cwqypumm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hbtobpyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2doicegfh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2knbjbjql.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxlobqz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nguiftqx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2aqbqquuj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2texvecnd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rojfqdgg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhwljvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkehnkmb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tpopdvbi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2klfxuldd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2oyqgzumh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xpswuhch.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bmzlrkkp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2omvhvzdz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nmlgsagh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2stwbkkzh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2krhqwhdh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2enryjuaa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2blimkhtk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpjngksu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjiuuoat.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2igobzaso.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfyhzxlt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hnygpskq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pxjhpazm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2olpmbcbl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jatzxoer.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xmpxwhcx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dggxhuqz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2irnkvcyp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tfxkrcgd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jjiqutpj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xraroniq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycneqtoc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2otetzrof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zdypupgt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nplxpvjf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vewooemb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fadrklih.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ydertffr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bydklxck.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hterswkn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2igjftcmv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ieelrmhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpwhfgq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bawnsays.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zntgehkg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2opqjamtt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2onpogjto.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2oisrtwad.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2amicqofx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxklruy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2diaghdxe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yqvhqato.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgjersnp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2afgbzyoa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rfoteqtb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2spaovbdo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2alhxnujp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2emyombci.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryddbkrp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyftronz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dltttocc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghvthbjg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2leyppvkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cjhrjnft.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zofbufvg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2axscdwai.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tfspllgp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wpccqlib.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kcmmkjom.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2etnvbfid.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zrqekftc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rdljmtot.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xyrvvbki.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixswejlr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zzxsmqhw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qmaedfll.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bwfkutwz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vrztownx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vqnnooug.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ytcccbde.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eibkrazf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eapknagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gafabsyb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zqnfxkje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgbmgsru.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hbgkizir.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bbtmyknu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hblulfmn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gfgbqddu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2diroyvuo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghbjikdd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yqzilghr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mahtruqq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mzzcmrmh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqcszkeg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wjihcrcc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2odtkuvic.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kegytslt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiizblzu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjjrkyr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nssfafxa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2atsxcsof.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ibqjfnse.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vbruksvt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jgwbxcuc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mvotbxhq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2itxuauja.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dqjjhves.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jchpdkqa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iezbndux.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lkkmraau.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hjsmmnze.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mkxbzvhs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jjadbjfz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mhtxqpyg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bndztglq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zhuwovvj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2heqgijru.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cxnwsyme.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2enttjssb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wlpcktag.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rqvvnyqq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kupekwum.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iyamcbyf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csnfrrrc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gurktmyf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nsklzlug.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xrnilsnt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxagldbz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykyvzrek.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nurixdgj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odwwjvqs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xbpqtolv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgmythes.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2feweviub.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fyqjrixy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhfyhjmt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rueidpud.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfkpjwlt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2etnpuenq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sgdwxryu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibrjffzs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jnescimy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pukvhjqb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sydlmkqz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hgrmsrwd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2crpmkaqr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hssutnla.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fzrxuzvh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oaojoejc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tbesajbs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tslqboto.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bhrhzbsu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vjetussg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2iaekggik.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uiavvaev.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrojkklr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fleyjouv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yiglhdvm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odsuflqb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2csuxnwbk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uvfxqxnl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dhkzlrih.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fojqqfsh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmsqbhcc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fjzklgju.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lurntyok.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdudehdb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rffngobl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auhscyva.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovpbdngi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nrrtlylo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tstqgcck.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndzmsmch.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrgznpua.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wqximfwn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oosebkpk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vmlytfbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szshgaww.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pffkfmre.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gyrfbety.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zqqlxwdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azhuogpk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2loztmvjd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zkpczqrb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvumynt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wsahpppi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nrzjaunf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rnefkzbt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jttwgwbn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hxyxwuos.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uftfzave.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hgdfuiil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tprmylbx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tuetosko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzffdtfm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2adjszddg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vfbvdpfx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhojkrty.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sgsqcfmx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdfgjolt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kobwnzeq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iybtephj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sibvzhvr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahsudytj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2avwtdeyd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cogsmuin.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vrnzmmtb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2phpzdnzj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxfgschn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udoyogjt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ynmymtob.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoxjgkfk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xithfazc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2whqjxhrq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2axgwmqfq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yzgrsrlj.html


<!-- 参考信息 -->