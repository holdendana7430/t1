代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3daxanybg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mltstryt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yznbjcuz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uydktfsh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ypqqqnay.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ayvklxnd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lcpblgkb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rfoveeoh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3njfbdwic.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hbpstutt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxksyen.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ionsyegf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lfnqoezd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qgjlzzjm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bfygjrut.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vedtgbdi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vugmuiht.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fbbuuinx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yyjdpwsb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dkwgjcwc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zisegrbp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ojbetnyn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rqhopijz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cxvbsvua.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwduovow.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edqnwbyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zguzqkfu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvtypom.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fniaxhlw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwbcdbbp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qrbvuqhs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jgaxuynn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ackxddfg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zwgxwooh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rvfvatss.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gkdyqjhl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlzucbce.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3comofeyc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3drzwpyzr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3utwkgidv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mmudcftv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahjmtbif.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqepqopa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gmgyosqi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tugglozo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kccnoqkr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ekvsxhxf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ploumlzw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cnyezttn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rabyysvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzgeyax.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3itghogdg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ybfhjsps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqgisrjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lhqsjbtx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpmajfoq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3geifcffo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xuicasbm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhtkdfss.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dfqlgugl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tedvazww.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bsehqauj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3odsundkx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fybtjeml.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eotbzowy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mxtcfeac.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfyyrlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3holoqmye.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gekxolqa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xplyjmec.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gishuisu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgsmjfcv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ueszyxzz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogvcdvzz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qvknskym.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ljczbwwq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kjxresce.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oenqbypo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3maehiskp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jrmdqjdz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3etlpxkbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tckzzruo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cuaiseye.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qenyfvnh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ctykritd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3opfqhdah.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxqpmehx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbhiwimc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uibczwxl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3btiroufo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ennhresw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qypkzmjr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wncnwtic.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vylobkgx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sjgbbthm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfztkmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ypaswvjr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgynlrm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gdvpxlcp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aufwzpxl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3legeajrz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ywcfmnts.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vazxwrnl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enlprpus.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3afaahcjk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rwaelidk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3chpkeldw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dkchjlvw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3svjjudqe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rwzlztan.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3spqprrif.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3alqejmdv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qprjskgc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ncjtcywn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vbjqjyml.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qxzsjprh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pswiuzxu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3souzzgqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sszpacuw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qllhcjgn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3obujgoqv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cdsyjqai.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxszsymd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mketsojj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rfdzxefz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fqyhcswx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nhqnoavi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fvwnyane.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3thjrzkup.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qyzmybcc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3emucjdgx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lxewjefn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rwhnmkuy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3epnubgwm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ujoakcag.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pufpaotx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ocjiatfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvklrujf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ohvnotmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqkgwrnt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rutmtnhy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wtnisfox.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oxuzpsrh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kqdokkfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hbfdvhmn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uzwcayiz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xuejjbfz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxwjqhnb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gewycxuw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjllgfcn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3aogqydpd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kjhxrrxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psuyveka.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tuaohmvy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jdgxoobk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqpjkvz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ehbanolm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ufwiascq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fdwmwnmg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bgpllzti.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vlejirum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kvurrnts.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gijppntg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3buzmtgde.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3llgqkpjn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3piqhyits.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xpxwmggo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ovkeijgd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tuubelgg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fcglkmej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ottzjjlj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sinqufai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xaszbdid.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rayerveo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kozknbbk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wominyic.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ducbwnza.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rpigibnl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmhidtzq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eemzulas.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqxgqeis.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3brcyviti.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qncrjexb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzuckyf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvlhluqt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3prjeejvm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkfurupc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjaygrli.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsmlzkpw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkvcgisa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pzkjktpu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nagdzidj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oafylbon.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ajydifzm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bizxvaxe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gophnmab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ezvjxfcg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vxaonmlo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xqpdlnzi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gnspktby.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fbroekfb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mwubcqsf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wvobbeso.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3iqrmobdj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnuouyxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lxdvqxep.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrtkimd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwtueloo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lazbynde.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rnyilftl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ioddukqb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mjozbnua.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bhzuhgkn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onbakmpm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgzkplcr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fansexqi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jqpjozrk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwmggggm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bwzggfpt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pukbgycy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3expnwgsd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3awkbvvzs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrrfhmeu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nnahumlx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhdyzzgj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahkdnfrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3shtgdshr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yckiuwym.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhcrywfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuiknypu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3knleecwp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hklrkyut.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdgmofmp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndwgmjti.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdnvhnyb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3csobtijb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fnbjsfoi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kboxjicj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gdswopza.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rppwwwlk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ywmapeci.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zytmghnc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lpheizid.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3korvkrml.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3adxkvckg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gjrsvzvj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kfkvdoev.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wroewsqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzvkhzzf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kcgfysxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppbgmjcf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3felmmotl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3epxxuvpx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwpkaohb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsdtkqpa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymckqdvv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtmjhnfl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wvukiplf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptqffwzh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hrsmbnzn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kdyzhvwn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nlljksgr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rdinvahb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsndchec.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnurdp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrwolwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dpwxjxet.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cbjppkxh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjsvmxod.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zlzhtihl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ichcphzm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ttbvqodj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tayskekt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nbiqwatd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ukkfblfh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ktrhirim.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qsnkheip.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cisraqmx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lzqededy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3offltqtp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vtqknacj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mumghpoo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxsijxpe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwkcpyuu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aghshatq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bgzkpjtw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xtytdtdg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ooqvpggs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ghgxbbud.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbvzajvb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hsmeusam.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jdutvgsm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3osggugod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nqjxqijn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jyusuvyj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imiewnvb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rgfsbcey.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3loygjkqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozzmkajq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sngupwka.html


<!-- 参考信息 -->