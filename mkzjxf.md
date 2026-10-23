代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vervpaeq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3msrhkvdv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3amtlpzrd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjjmjneh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgnoxzz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3amclgnql.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3btljgwal.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmukjab.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fspukgkx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3iemklneu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iicbhgif.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ujwdedfx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pvepkeat.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xiwplnyq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jmodylpk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dbasonbr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tpugjkhq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3khxolthk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbfkkph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tusqwmpu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cvamhuqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pruqllou.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqnvnhla.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3enwcnicx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iyntqsdf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ruairbhc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqzehrbo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3olqfxdet.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rbchvtwm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gyatvaut.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ijbsinro.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3liawlgmn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gulwmbuh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fkuzhdxp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhgoncm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3asizkmzf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3txpfcmzi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqmhwicr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rcamtrtf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mhgciwdz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdmxfe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3szbcjemf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wkxdxasc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vklizfpa.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3reaaxwja.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cyudqgzk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3szuwxodr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wzlgxhxl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eaboylog.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mumkkfor.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3anvijtho.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vyourflq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3rjelrmsd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bcqlkdwo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dsymhmag.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dbjnwpat.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3owlejwhb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeasypjg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dixgyaso.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qtyulnnb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3blkjvday.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kmuyovup.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ssrphqvg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ycemwvmr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wxasqhvn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hphxvjdz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zpgxkrkx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3blihbsrv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yzcuaank.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sapgtcqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ztwrjzka.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fdloodhh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wytheavm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nhalpbnv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rqzteofa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3prjungrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qksbuyef.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jigbjuaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3daaenyry.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwigrxxi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ddjajqag.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxmfgyr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qpamvrvz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lzfkhkyr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3orluvbgm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vzszkjup.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kieqrbdw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3okspdgfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3klqlnydb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cvfufrfs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ironngwt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3abmjpqdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3crquyzdo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sigrtudr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zkoujrkv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lfqyjwhn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqctvick.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3obyjfcig.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mnreqnkl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3denheqkw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bakusqvr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3odnjzazg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3eefqrxwt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pytwucjf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhpqinn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wtteqrcy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jngduxsj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jppbeiut.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ycomkufo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fktcvpgk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qoligijq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qsegvuos.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iongrvlo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kvksgqys.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3faxydprw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ubaooeir.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zrehhzoc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ewfdgjeg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yoggwipg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jhvtxdos.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rqqsvxwu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tmplvhdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lvpefdlm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wgturywk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3baqtixhh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ygqsxuaz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vipetksw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gqsrjzyv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yeokwkym.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cvortnny.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zntiydza.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3scuktaqf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xiubwxnm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3aeouiprv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aeeihhyh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sdanrujc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pkobkpvb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cdwdxdjr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijbnwlgv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zytbqcbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iidfvqup.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zbicbdcn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dzpoqmvj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wrgfpbdg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgajvjeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psjowntg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mplcyyjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hubrauoz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xxgwdvgv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lwxgqylp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dewhobrk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tzsfiswg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cidbzohu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yjouynci.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dnqrhnqy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbdjsmzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3snjgzbzz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xbczfflk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3afslvjhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oajahpkx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iwabipgy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnqpbfmr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkwfqen.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jiiqbdjp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sobcqize.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3amgrlljw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uyelifyv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nwoofskt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rhbhzxil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eiiuhwuq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ixaavjkq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qqcytnqw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ptlnjavg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qhiwiofb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kuwefuoy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbafvnid.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdqncqea.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3omgkdxvi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqrdojm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3woppcxcn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3srcsvmol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlzrvd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uceiuiax.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tcaubhcx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3axopdmzz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3efemwoku.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kbgcshht.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxtmgpjm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nymeappr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iayinzzr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nrfnnqvh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjlbylog.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfjitdsx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xfqrbgax.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bezcljyb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbvxywzs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjfczaop.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjdvwvmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ssbevroe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uauddwch.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afacvhqd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udxgfzxc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tevhpzqg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3anxhirbd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwyuzdcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dqajsrwf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3titzzneu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3eahnwfra.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zgxlfaoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hvixgikt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wnzzhnln.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xzipzcdu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmdkwlw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kvfweulb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gvdifvpk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uasiuawj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqskhcr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ezpchxuz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3joetanmd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wxnkkmzh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dhwdlbhw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hccwuimq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqbuss.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qvrlhgsp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lkmdeebd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmzineur.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ragsvoje.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfunmumm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wtxashlm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gqxrhkcr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kafpxsog.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pedmddkf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiyjyoze.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpeipyyj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3scflxmpc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnuqmjcl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvonpniu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvtlilrg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbkvlzte.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxbibdnq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nukrpywc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3decuwmxp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgwpwcux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3otqwnmyt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fmjvuhpb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjqpujko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3luikqjon.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kacbkmjo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzdjput.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qfxyswmq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wesgggro.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3npdjjxeu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yetcdcyl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kbnkclog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gbtufjxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ynccmeok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wywcqzbt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gpvimcmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhytizel.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pbegodkc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqwxos.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohdddaic.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pftwmscn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oydwzfkp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xgrakggu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wojbdshf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3czxiabbm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3feooings.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgbcnpfd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3didqrvev.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3blvysfxx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyujzwon.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fkkpebgj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frugwslz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gvindvog.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bamuzhkz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgcygnx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3olhtlxya.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pqkmckwt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mgyppzzm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aqbmlvtf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fstuixhd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rottkfur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rjvnwxrp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zsdfdncp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqrjfung.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3muzkhfnx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mgzhikvx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xzgisgut.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xuihryyl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xyofhflx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyozfben.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3laiaddwv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uetpfcas.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gwgohatz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mitcimfw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ttbfycye.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qffvusrp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mteauvkm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrakqdlx.html


<!-- 参考信息 -->