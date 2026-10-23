代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rfgkwjix.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3txspizns.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ajmognzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aiyvxool.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjtpjw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3epriwvdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vtbxvggt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rulekwko.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fjvmrile.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xsexdqoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3scasbvpc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lagxfzin.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fyfklbky.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipewfndl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mbfeekid.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vlysjtlt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nbfiptvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrcvbqg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jeonxsef.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cykqapqo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ymgogann.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pvsdpabx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wdpgmyuv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqwiwlfg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhofyt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3netvdyre.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yntjstbt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chunddvk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rnjfebig.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cjcyhwwp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3eelfaajq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ebexewze.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vqnfgheg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sxhntqyc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxgtdxhu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdxaogr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmdkhbc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zuyacqcn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bedotazu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3whfodzpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nurqelqj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmmrnctm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nmjgkhlw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kfxaugau.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3smbdfbnn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wtrivrir.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lksahzln.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lboktdwo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jtjrspre.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ptxkzsus.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3chprcuhc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xwfzyofr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oebqkdfa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhkjfxi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wqmqpsws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nnighamn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bjzkrxiq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ioqqnusg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wonxenlj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3thwjchar.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nblilznt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bgzlldaz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ulbfujju.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yfimbdop.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xiuidgfe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dmcfbvat.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tigxorbl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oqxmvjbf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qhzcssbv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlipdkkr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejiasgen.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3slcsgtfe.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3narnukyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jeysxpfz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hqvpjugd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dgmobxpb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jrugnnyq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dxuorfza.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3crpmuvfm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzaaecab.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xwlstgqd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qefpwuqv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ahelddck.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dcsxaqzm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3uwrewcud.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qowkhsjt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bdfuzmxn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3drbnsaqf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kaengbzu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ugygsefg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3eumnfmjy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yfyyirur.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ylojdqcl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fvryflvg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvaydwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3liovavrp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dgvnjxtw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yylnoiyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bsulcyhl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3iijkybew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ykcacigi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3esruawsd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cjxenjnj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzhcwbvn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3asdxwdlt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ysjyqyir.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jhtvidcj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3eqayatpf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3swfnimui.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sjtewemr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yodabtnf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3aqidxugs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xtzzqyth.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3smjetgpw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aejvcyya.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ebhkgvvk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnmixxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxnsindu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3veaxttdh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ktbyrqqr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bzpmznss.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iuksbtru.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3togxhkmp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mixfzodi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dbzthrxb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdfrfyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khmnemjl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hmpdgsok.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fyxhqnkz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wocxbcyf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ydgaqltj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3espgucae.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rujsqizd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xhilfdhh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ounrvvvn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tmrgxrva.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tykkuczs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wlyewsvp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yyltkcug.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rypkmwxl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tgvlfpid.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otlqlgio.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3otkjjbwl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syjioiou.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3peixirdb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3paulvqry.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btylyocs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cegbdidy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3epvfzwpz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybyhtqjj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lecspzkl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jjoeejhj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sfiuqpam.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eaugdiuj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dufobxfe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sjcbmtel.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvdqwbqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrzdgrn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zdlzewhc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fumokzvo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zyqwhfdl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hkdtnyxd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qqtvtvkc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zcrakjfz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ucrzzylk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etysserp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3voulgbno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bywloqkw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fviauciq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vrjailqn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkbjiaco.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xulhwmqg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bjnlxnis.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dgfwysct.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3eojskmlv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fftjigsm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owwtpwbn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikcpxvbd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3iixveiph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mveddznu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ceqwwqwe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ogegqgkd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3drbihism.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fonjgokn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wgwhcxho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdywidae.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pbwepqzc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mponpimb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gybqeays.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kggxfphb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fyleuuvc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rsxrwaif.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dhilrven.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wmhpjoou.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mwrpftvo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3krycnijc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qhmrfsio.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yrrdsriw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3svnlbxgw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3daosajsc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3onbatxdu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3asxyloxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3emgwnzqm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3saqegbaw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3chnnaumf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aqamdlkk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dwiaemmx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vazkkdvf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dncdplfr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwwkogdn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3prbbomrj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxasapbc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syiunyah.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgxeut.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzvhvuwa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wgatpcpu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnbjhymq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrdraxry.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bznxtqnp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3blacjvqs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnolwhny.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ealzwfob.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cmakgugh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3siegtqrq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogfcvsbf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3snpwkbhy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mjjyflom.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbzouxhl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3admhklne.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yunoybns.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fkxvajzv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3flevzqil.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fkbaqyrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqgulfur.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szrwoeui.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kuhlugta.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pdlzevfx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3scoltbtz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ffajpvvk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sxhrwfae.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jgeeymgz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nymokmya.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yenjgbkq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mkgrkkto.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tkkwtmue.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvprvszv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mhjduehg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fifdcqmc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yxihhhtk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jcietjqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drjesdtg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jircmzrv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwhniryz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqgbhsrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kbiipyyt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tapvrjve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlskrhjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztxqzpor.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnaftnfk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptsnyfuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajdynkro.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3asaosiyv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zodipmaw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3clvenmoo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3orkxzfcv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovvldcnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gfquiqpp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iayqrpoz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jgtbtwyz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3htifjods.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wucylwuv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3witsldlc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3czlxevub.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3holrwyxo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3suyxtsxw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ueeeryvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhilkvst.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qhuztqdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzdtuejs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dwcqhxug.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sczrmokp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgycozfj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iovymdgc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cbpldupd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rltwqukq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hjwbezrg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3riwnxnod.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odcycdmd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rxbezkpj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mrhujlzf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubraqjxb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3apccsbtl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pmzikkof.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxowodcq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgvhhon.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eylvjufm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlbkorr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3exlkcmsw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zvynqyuu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmzvemcb.html


<!-- 参考信息 -->