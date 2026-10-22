代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ofhvpelb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rketvfgt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oyvrmamj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2prrbhvlx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2almimvkc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gnlqppqu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nookbdrw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2trpwmdlf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ywuhwlzf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2uwsonsei.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2huaphzyl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gyuifubq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hpcaitux.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ixedzmik.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rwkdgjfw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngbwwehx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ivikahib.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2djakgetn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2djcprlry.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mnusqeiw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vqozjyuy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fgmwhlmm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rujdojfy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2clpiyzar.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2olbregjl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rpszwpwe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yqfitfqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmbkdkuh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gljintgq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ohacfuez.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gsnmyzgw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qgtvafww.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vbwvifqf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ooquetsu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yuezxsiy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzyljoo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ublpkuat.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iavhynfy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ernwpoxl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hdohhdoe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2emhvgxkc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ervhtnws.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uzsenmfd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2visqcpvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lgehmyly.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yjlffccr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pzastiey.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qfwkqzaj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tvdjkide.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lnpzjwwn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fhowlneu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2enazmtri.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qbwvklth.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqzohbdk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ucliuzma.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycubifpt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvfaxlow.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mfypcksf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tpujsvjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wjffaqqr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sdzehsae.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2auyfphwh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vzczisij.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgkrvfup.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pmnmobfx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nvgcyjqy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ygykdayu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ttskghcj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xmbeykfw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wlyvfowa.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wmyhmrmg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2asyrpurd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gasztyjq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gehlfhmp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2frbfywnv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bwrzmoyj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xtbzfdoe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zuzeazcy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ovszofgv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ctuvirkh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vjznkuii.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwziebfd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wezgwxbn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pmixukmp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ovllklml.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxjpkyet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xycctjho.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzprhgi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wxaohwnp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uqjjwikm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2sstbfeyc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpzxnje.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pvzmpgpn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2apfsxkqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hanxtrbn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2aktqhsho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gombxppg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2thutdpdb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvydhsh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvldxu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2luxfsrub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wqmdtfxu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2smdefozs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnpzebfu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnafrcq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkxnwpps.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dpsyiojo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2muknpouw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkjvzcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yntgcsoo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tvczgkab.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2otbemhtp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2znwpofbj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pxpibyrh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xjcxxuxk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjtorf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yezzfhnm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bkbgplzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nubhmrgl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wisvynyz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2awuigspc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mqezsqtp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2edouwfje.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dkgsakhf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfexvcmi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rjfopviu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2khmphyqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjaemsvx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ffufzzsp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uqkwaibr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaiaxcg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wlotyeir.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2inbpchgj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2coojzyfu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pqsrddek.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yxvfmpzk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bstjbgtv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjjmmyw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bopzintu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2syuplwgc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gdjladyw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cezqlnkl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rjepndbi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nlptgofy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hnonmrnv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeytfytb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vwoiqyis.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhkubvgx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uehakhyn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2auawbzeb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2leokdhwf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vrbxfvwf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ojgvemiy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzrazq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ewsdnmvo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2exbfiebx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iwsjrekt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wdzbywtw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2swgsbcbf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sebpuqnt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ndsqbktp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2slnnlhqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qsypviuf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2slalodpp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mqduemcm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pndezzjq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2quhidbvz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gltftziq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hmbjgblr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyulzrck.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uocbenma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qatrmkec.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2iddqclrg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2htrobmpm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ocokwnws.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2noenbkea.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ajavhval.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hovjehru.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fhfwjvqq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itogluzi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blmzygvt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2euepbcpg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2awtwvuxg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcfpshfr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xcjouvla.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orxnlgdx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sgmejlpj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2bkwehpcl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fjzuoraa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsmuthgt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qeewcfvk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iiondokc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sllbntzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qnqxezjq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fevjmjqs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xreadwri.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kejuelbh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ksltsdzx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gkyxsfum.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ncbxwaag.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oaquoehk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zdnslsvp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nqyvfxdk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yfipbnfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2brfgntmh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ieggjxtm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydjubwtz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hbphrubp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jechqnol.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jkmizvzx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxkymgln.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abmzoeql.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwlkahhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvnymqxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgnshug.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sokbwdwb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yodrcwfc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cndvyrel.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvvlnocf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdbmsoxa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdfwhqeq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljnxsuce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dgqlcsxz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpcaahj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmoxxxkv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyorwmkt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gclnuqwz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwiibeh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjrdgvm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sjeemfti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2runodulp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qppwgrac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yeprgmhj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vxmupnrs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ocpvelds.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sqxysagg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2voxikzcx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tubvvrcp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yakemnyf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ujduoczp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uhjxiymr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qrwnmtkn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pyyncstl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdrhhhia.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhprbc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oayqngqk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmyzkauv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dehkxdvw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2crmteglz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozbdmnmx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pggoinsz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eysvgarh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wesstlmg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oofspfln.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlwkrfrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnkinhxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjeehasj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfttxzjo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qjybeolm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etorredb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzireshk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydyajxgp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zfkyasfi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2inwhpmba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bwcqdtpr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uurzwvnf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgvcnnun.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qpewumkj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vjqclubi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eajokvwt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hozgyetz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lcbroiyb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ofnkqytj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ivzpctck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ejubxnsy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pnrqwvhl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rywcnwit.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wdfbmbwg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2eehhizea.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ubxkmgij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyhldtgu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ejsvlatf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwqoqspw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uhaqssyo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2withmzmu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snukkjui.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vvakqkua.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiycwpuy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2epsijtho.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xqenovbm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hbuqkrte.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxsutcgg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfxzsany.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cutlkcrd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbzaubxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fyfcqdol.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fzwcnmba.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kmatozvm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ucnzmevn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2whbsvmyp.html


<!-- 参考信息 -->