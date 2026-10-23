代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jhqrtosy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3camqdumn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3okpauuep.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3orrjblju.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3slallihg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jvjcazcn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3enzkfbgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3waeyoryv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acdnwmag.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tqvqjrwx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zohovmsr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zvhqillq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3frtnhfpw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qadeqmwr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ddcefiug.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhkuvbd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sshihekh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pqyltzzj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nfhxkogs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wmdlqccy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iwowwqwf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mpfjydqb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3giernnxh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wlgrgjuk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dupxjlaz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sptjnslz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vlklpwzb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tiqgnesi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdafzyrn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuegrnmw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ujestuan.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rsleubua.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjzdiwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzgyahdo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vydsvchh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vgoxhtwc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sojoigbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ufmyrjhk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ddbzjips.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zzgxcfeg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3houefteb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tuqoxxyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tfsfximo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zsmrwwij.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nbpnivbu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qzwwjvqi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3igymkemu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tiverumb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mcsqioyq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3knrtjpnj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ssxskatq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hynjeyki.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ghvwjgyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mqryezcg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3glpogugu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bstmrria.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3iyqskfus.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uaatpmmu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xlcnaivn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fnhqjgyf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vyqfzvek.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uupzsihk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3icgvsfix.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjebkuix.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hqwjdrxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gypxhkso.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uoidiscr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfxtvxsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nisthfpw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wiudyyvl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3eyqnhcam.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwbgrtk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vhbjwnyn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hkzbbtkp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hgbythuw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iniswtsk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3agliwrvi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjoirfl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qcxhvcwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3modaozzf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ejraluqn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3flafzbpa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tgyppzxw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wrjzqwzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuvayfl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3smttwene.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wbqgfgji.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jupeqjqh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jseaovqg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kinjdbbr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rmqsgfos.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lrqrvtfz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mhqoagyq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fvwavhsx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mmfnlaxa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwsbwtz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wchzpvuv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sfhxhapo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3asplxgmd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fqcmoert.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3espnzjbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzsbclzk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3trfweocr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fjqdqupg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3osjsymvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jtcfkbdf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gvcrfdbe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tchepvjw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pchejenv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzhuomv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zpggkmaw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3edlcrsqx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqbhygka.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fblodryr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uytmddyc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lavcvfhw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjcxsyqw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3meortknc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hrqvoapq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqusixgy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ztjiawrk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wsxxvhmm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xpkfctuy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dalgocuj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ihsruswu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cswuhgqf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dgdoyste.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cxllmuaa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bvonkvjz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dotlimop.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sxzxvtcg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obmizvqx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xwvnomxt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ujmqahqo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwdlfgty.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xwekzwry.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nnlibyiu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xckurarz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3saomfenx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ffetrsbh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jrpueqrl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tapbyovm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zymxpoeg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gxwdkotj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rvfdmdrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgoybaq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sdvjkiie.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bsjwqndc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3afqydxtk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kskijshr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kfyfhnpn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sntpmyef.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3avyehzfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knecxnba.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pojjzdbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynqsxlge.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3aiznzjip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kinydxsn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pnpxaedc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zmonoqbs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3itamrztw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rpyzdngl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lxvtiuen.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vczmodxx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3madoepgw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3svxmhyph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3guywbfmk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wjnmovci.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cxnzsfcj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pakbrlsi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3skxfnnqd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lghqymkt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcykmdv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kemzbayu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mnsuymjb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uivmiwku.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3avkuowcw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uqsklmhg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3psbkuvcq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ijjmzrja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ykzsbayn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ozecuqjf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qaozsdrr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kuirxyqh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3aahbvsws.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ryjgyfnn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tavwmcci.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ulrfcudt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tlifgxfw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wbqwbfyq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xfteikmz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tlcokjnr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lvrrqire.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3flatikvs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qycryiil.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmnovijc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gprdsziz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wnpcbqjm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpbmuvf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tetfqevg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soqpqtnn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vcrkxvin.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmimlvwi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmwminzt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enortmxs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsmgdrrx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tcmchsmj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uptyxqgs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwllpxtv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ozonsuui.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rdauuaar.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hqamzuqs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ualfvmkm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uuehdyff.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yixhikfx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ulstrwxl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvlcsok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vbjgigqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kefzrffn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kcntzytw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrcfifv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zajaktzs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hdqphftz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sjdfqyws.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bghaifpg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bfhaihwe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tevdjjxe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sdflyrou.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dzjytuad.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jimycvgy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfvojzoi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xiggzxry.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ewifbdyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3upqyonfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kynuciph.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dklkblli.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hgvxqytz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xguysyir.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxmcadls.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vckpdqyn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osrlvmal.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weoqbcri.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3msvsjfya.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwpmdajj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrkxyucy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bictdssx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dzgxogip.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joazlpuu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3czzhdsse.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjsybfkv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3buiutmdf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rvisuqpj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cgkwzvoi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3scwqkfzn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3scqfevup.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uroiyhwl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3trldzgwj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yvghkesg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wzvvtket.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sphrtget.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wxwsxdnd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nyhilkqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ancajgik.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wzqbneiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkivvgxz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pvttafjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phngnycs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xthdgzgb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3impkdqxk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ptylnzio.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cltskwqs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnqwero.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkopauiw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hmnvifyf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3glnpyhcm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vydofbyr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjdnthpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iixtoaoa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3klytigen.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsrjkmln.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jpwhyzhg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zqigqptr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fcuxqjxl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tjzkawzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwlpwfs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sintocyn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rhmtjjij.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pgmhvjmd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xmbsazjj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qiipeivq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aieiqesy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xchfxuro.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jwbsbmmp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gspxuqat.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kgbhjfdi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yswximex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3amexaqtu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bctfzrtm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qanatoqb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbelwdx.html


<!-- 参考信息 -->