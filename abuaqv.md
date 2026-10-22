代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kefiojrd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gtibugsa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uiyqcbbu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wvpqvexd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2owgbanpi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qsogrkoy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2keyschub.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fwapkgga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dcfejrdf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kxchzvdz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nfggkaqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ahnxwfsu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aiqftatw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wlupsnec.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyvrhklr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2adbbvaoe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dcvexgtb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibpwdztp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bsiqxrqr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cyobxtew.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qgdwumzu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2afzkheqy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2azxbjvoc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cnafbfuh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixxvxiij.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mgksfbfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qdudiiqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxlugjc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fcctvocw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2msymebzk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nykozmsm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uaopirfa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2orafifei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nziwoeyc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hlllpedz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvehwjn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kafrectc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tvtmngnc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ncshdcbz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ugdncznr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gbdakhdl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkywnnbv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lfibdtfk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2typffgzw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wxeidwiy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdeqvywt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aryfqdfi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hwdbzdve.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2npmwiqia.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ajuozsuf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ftblhhmc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxfhosqh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2afxmsqaj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tadmtlxv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zktltkyf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gsfckcnl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2agsygplq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cekbnobo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nwlzvzjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wkoscrfa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jsqkmgum.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ovnostvq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zgxgeloq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sdxqikrj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ortushfv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onzvndgy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2opjjjeyd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2peklwfrt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aojgiqbd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wdlldvnl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2udnbqqvn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vkavwtlu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cssfyaqg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2huccxfzf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mohpwzjw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2najfmilv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zkodktmx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2isgkvxeq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2owchltxd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2onfmpslm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqtymwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rabopczt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2itqeigus.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekakgimb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gparcpyz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ktvcpvjy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ajxxnvjw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwyapfbw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pvqrcqnn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wvflavyi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2azvmhgmg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yexyitqy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lalpdlcy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vogpqmvk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hclyeesn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2flviityc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaezzlf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2solwlapy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtywcah.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kzhutmht.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gjnogdyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ystsrexf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vaxytpov.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbyxpmg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2myfarfar.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2exiojtkq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zhtypgol.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrqskiib.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yxauocfx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2royjrnhp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2atbdpwuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bnsswvnn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2naxdwenw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ywnmujzg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2boiomigo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2algqffwh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eulswqqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmkxfy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wgqngvtb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2obmvnfod.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iiovnocj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kfhakujo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2msyfrdxn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ontsknfh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qlkrwozd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jcyayfdg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2geygqcse.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjcomsz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2caeisdec.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2svlpqbga.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ryyljymj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvveeo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ujbkssim.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sfcwvzxa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uovcmcjs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ogounpci.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eftldksh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvrkfru.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yscnrtfh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hzqdizif.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hkayiyjn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mokqvnbc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2svyzvsys.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pkpsisvk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xvotnmah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbbjaqb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwqhfaog.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jtxivsky.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjombpeb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2izjbvbxc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2huxmgkec.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2emtsijjl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kknxsdwb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rswpewku.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocdorjem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uxsfpglf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dnwetfjl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bknvhmft.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ldhavrvj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2evebbmlk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ktlkflcl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zslfbqqq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gbkssbhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2byktjhnf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ipsjjomj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bhpdhcsg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bjejglfq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufgdipjd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mpxxdswj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehjijgak.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ejmpesrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqfwzpei.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndtpwvco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xuxsziot.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwvtczlt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pedohpgs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rzveqfod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2elmtwrge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hcvmousq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjuyds.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fvbeakgm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyjrbuly.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ausfljzr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dvbokfqk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqorxuzl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mamicucn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2axllgwzl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uyywlzzk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bresmqac.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yycnfkui.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ihxtuuvb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gmewdglq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dqiuwfsf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nxzvgipi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qhzvelkb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2voeowvtk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bjhmalch.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zazoexbe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dmliksea.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2swtwczdh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xgknezqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jpgevsnw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2glsgbnfz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mjllitix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qociqrmy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wopykjfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sifujfhq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pqzggysj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ksbcoywy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qmhxjcef.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cjkioqif.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2feygskgt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzchylhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2asedwxgd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2orepusbx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfklckjq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybadvbqw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rspgdghq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfshcxnw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ymwqqvmc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwdaroix.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eavnlqgu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2opfpnjxm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfrpssow.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwfpyyoe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzkkccur.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2npjgrzrs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjvhibt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jwwexrcq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2plclqpmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ojeaoftr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wcuklnyu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbtqdqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jmfouroc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ofdpvofk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2umzxkvnu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xidnixqi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wbtnmops.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vwziaatw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bmqwbucp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qjeebjkc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qlpinccu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2htbfyqjp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rlqyrskr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zgclyqar.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oioylmtr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2grsgvtfw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2upmhwgjq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qvwuyeap.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ktqivxdj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dhcgezbh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwyeohip.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rejmxelu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mwjnwqce.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrajdpe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmcokagb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwmedb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uawicaxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vzcdspgf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgbsfjwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szleakcm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykykqdvp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kfzqwlfb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvwsyqrq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epfjistr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmzuovqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alhooyvi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwsabjx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jpkamfhm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivbzhlhh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcxdbeyd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pbtyieco.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dbfxbalv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cukmfoxr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pyqkqbya.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2senrxdqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zsvlbdui.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kokvdick.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cdhbjnud.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hnwnulka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxujsyev.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rjfqednn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwpxkvny.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ekptakjb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zvhnrcjn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtudxwca.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2odgisdni.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofuegzn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqhleiry.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nihabbyc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tzyxglln.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sikiarix.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtzohheh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2znkevrhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjagvyhh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dsliplav.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyifdqjj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpfazifl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pktrvymo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jkltpmwc.html


<!-- 参考信息 -->