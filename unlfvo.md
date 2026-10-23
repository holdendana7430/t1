代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zykbriej.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ztphxzed.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3olgjsndv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3afrbqabl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xudnqwfw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zydbosmi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jtjdrfij.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gpdfhtta.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3grqpxrga.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bakkveuj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yskvartr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3imqhxehv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ngjvgigz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ysbwbzhd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gjglefcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3emibehhd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3inlslkzk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fvtnarxv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vjhkpvlx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcotkemu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cvzwiqpd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dsstrigw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oiybvxkq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vvbomodk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpznqct.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kzsmmhmk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyywyrvu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sricizru.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgkenkul.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3giupijtc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wovlxxio.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omfljmds.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sjctwkee.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3usluydhs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ylwizmvm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xklqrdwu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jblzvpac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3asslphuc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dcrryumf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uijudvnh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qiymxplo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nopqdlbs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nvtotwxa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3onzcdswo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pkeubgbv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xtwexntt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bmoqtlxm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uwnkpoyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kkhngiqt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zqesyasm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hvmeivny.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cuwoolws.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bimtxicf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3slkqhhtw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rsffdcec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3abhqijkl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3aohuulss.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yodukbhv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3aejhdtuj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ccobuthm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gromqwbz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dcbofqqt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvcbieh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gkdiciuu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dahvtgwt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ohjntrtw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qtzgdjip.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3orhfqvrh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hyozopoz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3syezcdlw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xhkrlixf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lfmjuulc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbuhon.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eruwgput.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pyhbdqcy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3puercmjf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qwouymyf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pgciclfu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ikfpgodh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dhgwbryu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjzbivl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jydqslvq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tdjcivek.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fliuavef.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gqkueflv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dguwdhpw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnkqdjpn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bytkcsia.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sirjivgv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3huwkdumr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjmytx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aomzfgru.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tpfhmdfa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cvvnvzor.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mwmrddgm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3symaerqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjtbbop.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mswojuot.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gdwdxaze.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gmrbtakm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vulfqtae.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ujxvpgex.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvjjedzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nvaecfjk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehatmakt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mlgaunpm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pirdpbac.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoeinhpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esfyyrtr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vovxtnek.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3udppqzcy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iisjklnq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mfttjffg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3woivmxkf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zaotwfhv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iqjlrjjy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mdgcbzqn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3afzmqfrp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3amvuufqy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fsdkysqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vicumakx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tfosyxnv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnonvsuw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3noeixcpf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3olasmajy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qpsnqekp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hsdeonvz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ystqcxgf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3thpxutvd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zagqjnbx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wimwqbfc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbyyghaw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sbgelsyv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rdxsltbv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgxbdah.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqllfepw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3okbelqwp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3adppdmsn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ebtqlifl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kltzamyt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aauvrler.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aelsidlz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3budhzllm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mshopjeg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kaiptlns.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zwlcybxi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eqfoourm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ihuftrqq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ahkvwcci.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xabwmawn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mhiapvgf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhkhobfp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zxmffwbe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wxwoivfu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qhzanbxh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3drfalzfx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jgnzdtaz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oufyzlry.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wbnuzbay.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3czyhzpyc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3crlimlaa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bxiwbpfi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rcnoxyvd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfyxpfiw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3eerplulu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zlmeqtax.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rtcfnxoq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lemokffq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xsakiazb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jqgxpxvc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yrfvonhz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lujppwan.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3buutewrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xurtjffz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ixkxkybl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uftcrzzl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvmpanqo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xknlecic.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pdctmtuu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qgwtvxcd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hryjunso.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3msinkyuu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qyasptyx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnbepkim.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xgalfhug.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeosxnjq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pvvsbqqu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ivobhhxh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvjpphwn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3peeyalsd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fizglhen.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3clidcjja.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zlxotvji.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qyzqxdlr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jzgkdkrs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mlpedrjz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pzqyyqbq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3omygfhlr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ibsjujjv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3meskcfew.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqjsdwi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3elymbdtc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nudytbub.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwciehvn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3thlbcdsf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zvccrysl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iihynhmp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxyhyzny.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3grkrxvan.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3suwlnmcz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xfwdmjmn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3npmjoprh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lxqxuxum.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3eirstudn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gihaulom.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbecmgzn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jucmwhbw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3behvezei.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dcdgnngq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwsruxad.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llbegbje.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nlctdusl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqetqtwv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xhbwsdtj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgavzfzz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwfwfufi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3srvqnzlk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moinedhz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yucicpow.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svveuoqp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bajqbkgy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3myncohjd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3biekkmxt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3khhvqpeq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3egummpaq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3okliugwc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpzwlvo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jhqmunve.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pjyjhxbd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nlgvozuo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uisjlfzs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kedewbqz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oaeyrrvr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3omajccfw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mxeqgobm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3piievagk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ouwblgli.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qblusgwq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3iizhakuh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txmqftxy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pczjmffd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fcomrxzn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hdgvohem.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bojehqov.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ybiagjer.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpgecmht.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3swncwlew.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xkibvuhd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vaopqtbi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpoagdog.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnbpfzfk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcfxkxqu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gkgncmqc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fviwoikn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrhvsqel.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlstybae.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mobebzfp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhdogm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tzejechk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3etrgopul.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhuwswli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hstludfr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pyyqcbpw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmvjekfj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ulfzgqom.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ufevsnyc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fnagadbh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uojjokhz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vyuwlrit.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cligjsya.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3omavnwze.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hhjhojet.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lfjtzimh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hltyhztt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilylwagl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dispxaye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdbsxddz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fvebejyo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dbozuyqd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gciydcjm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3haasodmg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3inieqqim.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxzkcmgq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3onbcyvoz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ciesbabn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xoiferkd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yyfcwyhf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yzodomdq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crklikkl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3befcuyeg.html


<!-- 参考信息 -->