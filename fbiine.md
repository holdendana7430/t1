代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mkuhbizq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ycwxxjcg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lgniifws.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qwyeqoah.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cxdbkfok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3szazfmru.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqniosh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zfkimrqw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3baykeffy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3djmzhqpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nlcmetao.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhmlxste.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ratnagqj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dhgzvucv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wrsoqqsh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hyaftgmn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nabazpww.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ejaijgaj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rsxiqxxb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gqpubxbu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fzzrlgaw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lsyeianb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kdpuukrm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfwrgnqs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bjeajvup.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hytrkgjj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tlxbfizy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3oyfjkldi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ghuujaxw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ueljszcp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ctaoumxb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xvoomtsu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xfpynyrs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uzpvudnq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jpjdrkix.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmyykog.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bgdibgtr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dpmhbcsj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zkcvolay.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dkgqmfsx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqaxkmh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jvxjsxpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nuiyecrm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3twintvzl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwtowhza.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqxhage.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzusgwiv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kzxhbabg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3juteircw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3svcrityq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rvaujbyk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crclgzza.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3copjbqdb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mmlbiqfq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tcnfwgpm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nlrkgzxz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kkzzpnqo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwsoemuq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jlfmnhxx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3czlpdgvk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3epigxxbz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vhjgxtva.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3aeijudez.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wkvfleqa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xeyxqlqf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qhjuexmw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xhrcmhzh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xqkvsvqa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3yhmxgsye.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzrqfzsj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gguohfnh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3eqycnmku.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dbdixxuc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vjueamin.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3asphxqpn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ctwwmseh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hiqedsdx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3msgucuwg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkpscnv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajpxiwcy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdkyocvo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sypjtwdu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lqwhnbon.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3herndcts.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jexbozjy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kkrhwsrg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jaqblvmp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bjldpaqc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qxgdweeq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3urburbne.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xhnwbugp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3andwjkkt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3elrssxvk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3enxgrqld.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uykqaqdi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbhcxycw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoycghvf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgwxblzb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pdfrbtyy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwwcbjwt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mmdqnuet.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeyvhbyd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3etvgeowx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwyibdle.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ouubzzxn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zqyxufrp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tqwvzrtm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qsusljbz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wnauwdmn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pfysfyxe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwhmcbj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3skiypjbw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jayzcpip.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3odzhebnl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3spevkyyl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmmzofaa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bcnvfwom.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mssburam.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3njyeezez.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pmlpcfex.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tixozzvk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3alqfoqju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3duvjmwmt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bukmqrch.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3itehftji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3plnizojy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uwasynwv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3eqmthonn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3whaeslui.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3plgnscht.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jbgeoeyv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yezlanqx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qoiobgzl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3abuudusk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oufpwnej.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytcikhle.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qmxuyjpd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nbvvovmh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3teflvwkh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3osrkxncc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xpuvipqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrobyugr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfygtzob.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nppcguxr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3otsafdod.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3numkjfpl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mipqhmpu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3espllzbu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qeyunsbg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qbjgrozq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fbnncfty.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pnkmtkgm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hksoxrot.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3oqslsdjw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtrigfsv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3emllsjte.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rlkrdvkw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bnormrvj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3swuqcufg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rkmwqmte.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tipegosp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vujwutrn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cvnhyadt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvfzbyhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3luxlwwdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfaxbiil.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ibizyvjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhzskxbs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkpyhgog.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vgpzgzou.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3msigzbft.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3reucaekt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvefja.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rtsbymng.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pkknssfc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqmtsinm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czgpyevt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yelqygas.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jcnsccsj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqozgam.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxobixcz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dtpvpbdr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mymanobn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nrdhndfj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhqpyky.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhhepnsn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3knkqdgjb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yrxlzylx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3caanxeze.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cfcrdvxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qhucortw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ucbjjagd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nctzgete.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lzdfbjxf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ocuesfuq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mbdlvquz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yxqiypzk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vraympgz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xsojfnvp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3whlxopsk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mltmdgbf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mjcxrrfs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qsgcafnz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eyjnpdge.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gjoaqmdz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tzilvamx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gpwkahdl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nepotpcn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abjthwke.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3glwsqghq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xplrgsgt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xulslpla.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bzittsxz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3knjwioga.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyrutlpj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tmfdawhy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aazoorqd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atluygue.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eubwxviv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3datmrmjq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaumohxv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bpoalrue.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3itvtqzrr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3faqfnqqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qbenkoor.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3acxwpraa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zpisqnde.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sspttssr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zicenqik.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fifaephm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bqtcgfep.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wqaeygyz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3inxzkidr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xkrmkdqd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3crumrebf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ssyxjjbx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xmcegaow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qdblqrbg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nenzxyaw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zqjviglc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3myhykrtt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qiyupodl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwegfddx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vvqfhrep.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3adjbzcfy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdqfpcot.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kyvjpvbf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcqfqmdc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dpjotlce.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nolgclue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgrzfmld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvpqaqhv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhwypyox.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjzypqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mgrzyzxc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxupqiyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jklhwzjd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjmhshyl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sflcztju.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eaumxhem.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nixcmpaj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sriynxkv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3miburwyc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xwutzvaf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qlxaaagt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3okavibow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lovlnrks.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ljpkqbex.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdlbnjg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ywdqacuy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pyujafgl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kixtclzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ojxzcgcv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tpyfhszm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kpsxbfuz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nutjjbac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojxotlow.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nedxuuys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldlpzuxd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wyecztnn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mnqzxnca.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3crclqcim.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rrzjtilc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfgprcx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zlbifuni.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yownodxp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hhafcgvn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmpewivq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hrfuqadi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3voeearyb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jywbzqgx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwepzpjs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nojruvlg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfyxfldf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xergjvee.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qolbzwic.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zkmqwytd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3sscoopjy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oovxrsly.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dqmpadja.html


<!-- 参考信息 -->