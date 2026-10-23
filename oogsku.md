代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cgkvxava.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vskvgmjv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3btewuahw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yvzcykfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qzqfplbt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3onnuwwvi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lrbwyjlj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lrjybrpf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3czbtrqba.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iipcbfgp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wolmkzqn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kkzdzhpg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zzpqjvrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3connnymf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mkkpmbix.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fxjyxtys.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjrolutw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tkhnebut.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vtbipieq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3curgqxha.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qexwdsrn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dygluvre.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wjpipyft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mpvqgupe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gqenbqpo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qurvbrlt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mpaffupf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3izwibdlt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3axsorqwn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3elninexe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uuxkrdih.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rtdyftkc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lddquxtf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3njerqzok.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrraqrqv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gjwsfyqm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrexjyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yggjwogp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dfcsngug.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pkzhwmhx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fxtuxsnj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3spqducyb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gbjnzfwx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3njgduzrz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hjmmtxcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bxchqkoh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vintvjdp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ovenbnkm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jilvkiel.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wanxvnuq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zmbtpoje.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ngaxziko.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3arhotswu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qgjwkhxa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ggbrjqot.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfqvactm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ilfvatvp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlnxwvd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3enwnpdmf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zfboajbv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tmvrfowm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ibpcbkff.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rzyqegpl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3imxuostv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wsbyixke.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3niaujkot.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3admmsobp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ojhffiqu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cjqtzmfx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjtnaqnh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmcatj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3axnqvmen.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xtplammp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3abzpgrgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wzklajou.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mwtsaybz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kriwzswj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgnqtmap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fbbecxzw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kcplsiml.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pnfvfmgy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ugvbxjaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wgvirlqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jzzbxkzz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzocgsfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3obiwvxzr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dafgnuda.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wkybyeve.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fgelgvra.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mdoetjpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpahijfw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3apelclbp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tnuotdzh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vhtixgmj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ghlxekbi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3flufitio.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bokdqfyi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uinilipz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pukwhhph.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnjnbvhe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xctusrbt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ufuymysa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xbaqekgu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ralqmnrm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kyzojqkv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kosoepid.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ozdenrqf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gppruufl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fnvxphen.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qjjnqhvr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rhxzimxi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wzefjpsq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kwkhjfxs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3poqwlhox.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rjejclwr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3awgoddfz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mgsmjmhp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hdyapazy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hdpdjrar.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3anpgrfby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pdccfgjs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkzfltw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3omnveewg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vpthecas.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mbflmexj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jbkepljr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3miolsazh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dyhnlygy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cqdjljrc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmyocybg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrjtijhs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3isfaqioh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jlqcumvu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sodcjufx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3waltvgey.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ptvkhzdh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cdgpxjyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujtiakrk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmxyqyyl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3csvnldaz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gucazdbz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kxlixspk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaugtqzy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gwbxwdcb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cmswhljt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eofkkvyy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3diepiuui.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nauytjlz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sfpvxtlb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jdozwgna.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xvopzjhq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qpeyasqd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3quszodzg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dfurwnhw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jempwuuu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qipdxvvu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yygesxly.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xfxnddmx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cngjnxwk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aogflicm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vmierfsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bztjlxyh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qzfdtxpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miqvyznz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3irpjgshn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yrbjyorg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmxrdebz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cdasltbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3prybmpzu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zubqpfrw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3oqwkdsnp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctcdybke.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzuhad.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fbxsqadt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3btwjnwxl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzedzojx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wbjpmzze.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kaitfagb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fgcyaljo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uilfljxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gactrmux.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yusimrpz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3flnocfim.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jftvvgwb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zjhundtl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3llrxsqww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jgclpwni.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ruahpgfh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxsimee.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lsakzpcr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3utyoxftw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3viupkudm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ymlfiuxl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hshhprcr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lmcbuydc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3whzmjyal.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3exjddxlh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wjsurxcl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cygqmiua.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3mkurzcty.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ywevdbfq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3stepvada.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmfzuwrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlexiqab.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juyuzxcx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xyqszmjv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzxfdwb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzrcmnvx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqjnuejy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptkerpdz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzsemrvw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onugdsxt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhxxpnuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfkbzojz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nnfegudg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqyzuias.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yndgpapj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqaazfxs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hiywtlnd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pemaafuy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kmqbyhbx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iqllxsjg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nozbzlvk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ryamapfc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhyqxsu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mheccbqx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hclosdad.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jmgoctev.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dnxjdhkc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hunwptiy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3whzeoaph.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uprhrizl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpmkowy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wnvnwlmr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ukvbcfwm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cqammvun.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qrjqkakk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjxepp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wyowqikk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wmloaozi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ypwelpzf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3anynmbwq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3aobxjtui.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uypfbgxw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3saoeyknz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iuvpwdmn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkvoeubg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zythbxvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fyaftebr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypycxaea.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lxjqqljv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uujkmdfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pefybcdp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhjiltby.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qisiryfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyhekhxk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lnhaaqjd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhteyytw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdundmzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsuiujj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gyahihcj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nveprimh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yldsakww.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hbfbacty.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3chhpkqjp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xwfmrrxr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mlhuuubk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3raiagqys.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xmrvdtma.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jrwmpscp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dlylqhto.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bjzcfwlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfpzkuas.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3oydvmurk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaeaevsj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yeppeadp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uzwvvzwy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vstekyoi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3immgjgrv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3klahqcmf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ceclqzty.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3obetrrob.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3epddronl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snqnsozc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmkmpyuh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xijmxdcs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swyzasih.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nelvbujo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qklxbpei.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzecmkee.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3safrttic.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3htddgkto.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uedpltrd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fbyzidsc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3whrujpwh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mbfovlbj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cdpbiwil.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qlznjsqr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ssdujafn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kfaqynue.html


<!-- 参考信息 -->