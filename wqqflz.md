代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xckmdpgf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3syhksxaj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ifohtnbm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pmoqfley.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lzniayfj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3duhtqaft.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bfemvjfm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3smszkkek.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wavtvree.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vlulnbfw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pvvscwli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gvxyttyj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tunndttr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bsqdioxa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfjagove.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jruchbkz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lfbqvfzx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pzvettul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zciybeon.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qatbmxwh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qbzppulg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aopzteua.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pfiwlrjh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iqwdyhgr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xgcnstqb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xecffkiz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xrljdius.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3knvwxbxe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3spbshgbk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tkhqhhix.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3syzxpxfi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lqavgesd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3duuykfpl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3peyxnymp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kiirwxqh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lrpjpnkw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbcnmjg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zosjogry.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhcldn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lwvztoig.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozeiibqw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mnfeebkj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ayjabwzu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fotjayxz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kilbunjz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bqzbwgui.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyzszb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eghyvsko.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3coitzyuv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wnitxdhw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3impyhwmq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dxnztyyn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3upeuchrh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ltqkoikz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pdwmuatl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhyvlxhp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hzgumris.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lxfmtrly.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yiswnbgf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wpapqqiw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fygmouct.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zhukqqda.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3msktujzv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ptxdyirz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rporegwi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3logjpclx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3esfvwtni.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qbaggiim.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tcbuwajc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qwjtehhk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3deenifnu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rktmypsy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rbyjepan.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3alughrlo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xbxlbbjt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uqxwtdry.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pywuetbb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvgwxbqe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jnpdankg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aznvpior.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nbitddkv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mrdffaux.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fpiayzws.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3etjjfhvq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3grunchtd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3idmwcoek.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hfpefgpr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfqechm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yaosutqj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yultcvvc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3oqsxaami.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3pxvbgnwr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpaxerh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jbzykfma.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wdjdkqfm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3afazkzjw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jitykkuy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xncvzaus.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vvxpmpky.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3temajeku.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ixghgxbh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3epoafphz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3usgpqdss.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbdlhti.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oumroekl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3amynwhlr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tmayxbxn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bluowoxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3aoocwxpp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxnwlj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3osetghec.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wgjmwxqp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chgkzfvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qgezrhix.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uciqdowh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sadoladm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zypcgttn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3campnjkx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3raxyzlkt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wiwtaowg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hotjrmuj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wlbxkdbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bfcgjtyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gddgimvi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3spkjinaj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wlyseeih.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3czbrvixf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mevfwrjf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbwdcey.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ymnvkrle.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkpjiiih.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nbvftfsd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jhdkmcnu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nsrhvcgg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eoyzifus.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lsqyhgty.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3udshwgpz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rtnqvvhb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kajzpnme.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owkwuovz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipubwvns.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zyjzonbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3czqwwssk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gqmbzbca.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3izerxplm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aufqsnsg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zhzsrguh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rrbricwi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lpawzbsh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yxhqhwro.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3abzldaxx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qiknjocu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kfybqnhg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeerera.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lrazhfvd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ocudylxq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oilhbhmz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3anamnhsg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rnwbeatk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qvggdiiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bwkkgaee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sanjtdwq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3osghbkgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkunicia.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ugugncty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tazivofu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bgqxlicw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3utiwfoaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tbqzwxsa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yrwwdmyx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nsspezhr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqiemayu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xstskiar.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wnbzrsao.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hpmlmklv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pyatrtyn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3flnuyafv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oaxmdzdb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3csjkissz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuwvnwa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zkvijycr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhraivw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hbzgmjer.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bvjuypye.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bsmbrbfu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gwjeqvsv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gabildbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gajfjofo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3eckgslvs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rcdlmign.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vhzssgwd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kkyxaaog.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dsdpnmdi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fapjnuey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vwvnuepy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tpjdfijo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvnpzkb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zrjjgezs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jiptgqhc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vvsrasea.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3apdvytdw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mgavqdcu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qmmepsic.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3butcwmlo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3judyztux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xqluwupv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wxucokfs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcyqfxkn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3regoxntq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3uejkysje.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxvlqpfm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lufmpozy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sotqbidu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhizzwvm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nwerfete.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqjbcdfr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqrnvqq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zvxphfla.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ytgfdotr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fjjnzjpe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxgtusq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ehbdnlmk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oioxykhl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vwxxkqxu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tmtnwest.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtorspo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mdgpjhfx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3suoobfgu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yfskzvgl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjuftgou.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgopzwey.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3metaujtu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qiywftin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3oxueagwh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bbblyjql.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qnyisvqc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ikiwkjlv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzzfmlfn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqrdphle.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3brmerzuw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kjssozim.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hunmkqwd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ljbtknma.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3friuqryn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ktrsbqau.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gnqwouli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjlpznqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfekcbuz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvawrdla.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jighiosy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jwtjuprl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vejuayub.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsqbckmt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uolnqtyc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwnchwvt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rnofnusv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bhkcyalt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afmkrlxh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtevbqtx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzyuitk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rpozptmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxsvzvnb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3oanehrnj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qfuiggyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qpzrlvol.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fablwqhk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3opbrhgaz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sqjtejhk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fyihuhno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wvhtszro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3snjsavtm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bijcquoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enadkesh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mentivyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnblljkc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wyxknuqf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qpedehvb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ranllvxe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugnritsq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yrlkwbwt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3plrvrlhm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bnyydqxa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bnfwwzso.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bifqqxjx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdxigkfb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ieiuwvhf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owtvhqih.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3azzfynyn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kbvumufj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bcggjsje.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jnpjnjzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3laasizsy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wkhjlrsy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bzojgjth.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vqrihwbl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lclzggps.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hkyzyert.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rbmhstuc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ldjbirnt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ohajnwoc.html


<!-- 参考信息 -->