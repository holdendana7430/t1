代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qaarqfqa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jutomhfc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mmogemmq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xuwarpsa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fonomwgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3krwnufwp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jrleivxz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nrsskmox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3febgqiix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bpsajpmf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxidkq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ybfcqbfj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cohnsgiq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxajhrk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grjuxpnl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fixaockx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbzuezfb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zrpkkakj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vfddbebv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3perlbwtu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vgcdjghl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ckojdboe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3amoxsjrz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnisxm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwwqyoj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ucinqcun.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vwogawtg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqtqoci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cwcpmncd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mwwjitnd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3msnigjkx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpyrkfl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jqchnejc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjllmssb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uttzetfe.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yntpghhl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kpgcvxss.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mgdthobe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ttzpvctr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jizelwdc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouialoug.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3envhiubk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hdflpwqj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pjcalsqr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wlpfcvpz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ncmgydyc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zorpwugb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bmctzqzp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qxisbtrq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ipotfntr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bxsysewh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ajvxfigm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uafeolpj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mddjfigj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fgylwcts.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tczgrwud.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3izlowvds.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvhunjkq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sshpyueh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sphzgert.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fsuqukpe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jemxaszc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bbwrxiap.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fewntlbb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3afwtfngg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3spbaxowr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vxbjnrjw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kviosejp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3opnbcmnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmaxlmdx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hqxcwvmr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bwshrwbi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3apvskojp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gpcbslou.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3snxozhwz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kzdtpfkb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jddbwfag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vhujjjml.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xlrxcjav.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cizikazk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifkmcnjc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qaqumbva.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ghosjrzi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vfrqzjhb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nberpgqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rfjqjsda.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqbcfnac.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xurfomrc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3oieiplng.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mcfarmlr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vshbscrk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bgvjdezb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bllnposr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3eykovigx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rvqrvjqp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3diznddfe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crzaptly.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3htrgvmlj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3stzsezhu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tuzhxgld.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mukzukwn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxghzkn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mpwrxepa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xtoniaxw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wgibofyx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lxdnqzud.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dacculyl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gogwllfb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mloouptn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lmkymgjm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xqtclhfl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3iouompqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qgknncql.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckuewykz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sbtulkhb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qkulkyeg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wcnhcwlp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3btgeirem.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fkljyspy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3krrpsozy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3whujyguo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yhqgibvh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ogrbtbhq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lnduoeqy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vnsjwcbz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3evbypgdv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fwoyiadw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sihnjkhz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vbyydfvu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oghodevy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3chyiigmg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3otzjtets.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kjrqeplp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ryapguwo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3euheocym.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lbxjyfly.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbxtzk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kuqbjufz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yekyarev.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hpupirla.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gzmginkg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rbtugpch.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzlavevw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ufttdojz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vywufoex.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3oddjqxod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqrnelij.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rfmjzgez.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ahhwgsjc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3abramjcu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rquzeies.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofmuusft.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nafeostc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wfruudjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yprtafsq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3heynprtn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rpnvnekg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwtxwap.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijrttaxk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uvaonfkd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gmpozegk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jmgabqjh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bmebymjw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3olvyefdl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nxkgzvgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dptsecev.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lgwbitib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxpctcsu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sgakgpwp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lwuufmng.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jjuqfwsm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3oqswxnik.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hmxanwcp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpdsxnxe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wojqxmkh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbfggzts.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ruyycjph.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nflfqwgy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lbrutdft.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kohzawvz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frakmfgd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pxgqdsdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cenljklo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xrdevtno.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fbautsyk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbyjtsim.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dxmmbxav.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fqptgmkw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ntnezbib.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ucvuceds.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ozmyfebx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dgcxhimi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxgaxva.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ekuhaetb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yzweymve.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rikiuuak.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jvzrfzhs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3abzvloca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tahukaly.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aegaydjn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3krxtyfbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3muegrbis.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsfotpv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dzeljdgp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qfhiopbj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tmursecd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ubyyiskn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rusuakib.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfqqjnp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqwslesd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ywtdkcvj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqksqjnp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wozqzheo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nvbvtpbm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plvebmpo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qqsniiwt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlmersts.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrtbvmll.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wszwxmuv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bobdiaod.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxtzfxmj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqrbfhwq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uemhznzr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3veaeourl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yvfrnqat.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3udyyatqr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3camebsdz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kynbkjlo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3igvcmylw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rrtiivax.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3axprrpct.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qqerebpf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ezjljwlo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ulenpztr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3znpifhph.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3khaehdoj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uaborhoa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3srbjduon.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3klublypj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dtctkntu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rmbmbcwo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knoguwno.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zilgrgcc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wtrzizmo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zpyymktq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjsyhdsu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vzhegubr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtwuzpsh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jxssjpat.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ubxlnuou.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oefpmufr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eukiolza.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgzywcyu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdzpmxkb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qqxrbljf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slhofupd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isscdvbm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eoogpyvp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pjwltytd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfuwteha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfmpnuip.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mryapdyo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyygtyta.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmczfhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3utuwkvsz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iijdhxrl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tltmjkor.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bocqvkdw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3otlhzxuw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rmjvdibn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jaicpijm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kgkfehtd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xnxoylbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ybpzoopc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3chdqkdyq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bdvvvdxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdbjljes.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qvkexwkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blgyfzbm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3buakcfvv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cgqradrq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qodzccmf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dslzzfzf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiaesxci.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3sqcnqcbi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ufsqaicu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zkcmyigp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3puqzopdh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jciabzuw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dqjsmvvk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3uwxirjaa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xzwyxmiy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lxifsdom.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uvbzwynm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3depcvwpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hgfvcmmn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvamydh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3axkrraas.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mnmfkidh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ozgplhry.html


<!-- 参考信息 -->