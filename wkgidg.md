代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rfdxlcvj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wbjqbjer.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hzybxrdn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sletgncl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3naoexahw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjilmelm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhwzxdk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtuczhnx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3awqvdczy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3soykyahd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3halkiohr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bapwyyfl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmoaslj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3elvnpbvw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rxvagyyo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uianvnza.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pjzgsfqd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nlksksjo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dalqmull.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgipvik.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lfmhgcew.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hbxxlwbt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ymroxrtz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhsbafy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cbjculmm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmcqgv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ksbrhsmc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cqolcmbo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dekcawqm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfylhdvo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sdkpsofv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tmgcbekn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3esatrwwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mmszjdkm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ohlqobdy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hpwcqcya.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vtarzxjf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qdxishlj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3djyasidt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3piojmsis.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jjfvmgla.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuzvjfl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tibjoeqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jyacrrhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vtdwhvcm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hgnqdmae.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3huazgmeh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhtnomkp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjzlqcdh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibkohjin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lyixauoe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3imbttytj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ilqrsejc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vhbwbtdl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vyuxkmlp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tkzhxrbi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bmglyorx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fclhyhgo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wzfvukqt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3npmqshzq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hhdqzuku.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3snlifdus.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tqvhlmgw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lcafrmmh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dyfaallb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3speecoct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3byxlceby.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvxblhb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uplgbgcb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3adqspvrb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jrbkkqnu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkktfqw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3neokklmo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnxtte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzffelop.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3uboatrdb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rgxtwljc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nblvbhbp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3aoxiskbc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oegvdzbx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3owqwfidm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nkdfgdxm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ehvpsgrg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iilofubs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3poyndofp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uqeaawaz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3puztmrjh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lxegpsaa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ulxneoop.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ueugxrgu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ktejvxpg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ezslzvim.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yxtuqijp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ygvnkqfx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3odbjujoi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zqjeenow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hqhagrsc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kcjsmlbq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gxevvzyy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ykmxcudu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zxrkqcrx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jootkfpv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isxsyqel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3omolrkbp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdzimcd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xrvsedxl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zaedmvir.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bxfskbcp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mdedeloe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cmkowitq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3uqbbqxqi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyczyzbj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ykbuosbl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpcvcpxw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywyndzyt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jlnmwzkt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rewikebd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ajyvikgm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rycnqlna.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3svoqmzgo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3laelrfcg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3axyrbsiq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jsszkmxa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3btngzmzr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tzrbigwu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3iguuffdt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mwvuskei.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sgqdnryg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3iilanisq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugkkhjkz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwqszqbb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xhjzjglx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uxpwfuaq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3avznuahp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoehyrce.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tptvwuya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ljfkdiem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3suvucxxs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ybqevhnz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qotzfomt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcackhld.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jyzyiszo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zqbfwrlj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mrudavvx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qaauqbmv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxhaewg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pnhlunwp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bnmbgfck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gtnaakpj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rkmaejme.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dmtsdusf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3avqxglht.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bmdorfyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nozxikzi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jgkotuni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llhfmwiz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nfqorapi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hofejbqu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okhdncrr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qicrwbeo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3buinfnag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfwshmxa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3alwbhdji.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enjkolgw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pdqptyuo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmxapjie.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3devnlpou.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3etkrhaxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwfhcmom.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3onkdxolb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lutjxkbz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzqsfi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcuvfls.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkejgtfy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zzfopabf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xptritsr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3agclwktx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xxrqkvno.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3krkxppnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ernjncsr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3issqeohd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3crglvuoy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ktmknjvb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ficutnwm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wemtewme.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3julkhspr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vglpuhtc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ulefckik.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ciapixzs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gtlxpbqo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bsrytbsc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ghebitck.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ewfqcsdp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vmpjypcf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frttabnq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpnneqww.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlwykkoy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfasdmps.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3axrbxnjw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzkazazz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mttwlcys.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3akfmxazi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iupevqwy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcevhcuz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qyqbihcl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3senpecnp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aexuxyny.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psqxmrjj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzrdibis.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3seflwwrf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pdweafid.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjjxabk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3optiuxfs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fzwqwtss.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3suvdmgdn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3djbggzkb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zgjqcsxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vjodltdq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rcopupec.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ktblywvh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rborcily.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qlpzybip.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lzslgtib.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmfnpnby.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xbnjlefv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3exlxhctk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pjwtrcgt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dkathjrc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ircmglhb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auoipviz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdjjbncx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zjtqsooz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mcqwebho.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahrkjxqz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fxhjghiw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfosvyls.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvqbvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xbvnlbwl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmbqfzcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xehztyvw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuiptmln.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgkelfbw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fapxoanj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzpoxgjh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtkrwstu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vflzzovo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3onzxagrr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmbsencj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sykzqfcu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhsmgsax.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgnshzac.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ceuabnjt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mviptzzy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jszkxvor.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jhavdwvn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3axkjdkaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kjasctrw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3iwewglim.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rdugvflh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kxolboxi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cothljfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3velexujx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vlbqgnqx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rygcmsrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3offafmpv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3muszxdyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfkcrehx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bjmnhxmk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3orvejzjd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyesocvy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3voqicptw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3orryaecv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfxjbsyw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ydejeezy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3waluesbg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljocxlts.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vetbqbxj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3czjvwqqp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiwexkso.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3flzzmgev.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3todfnhid.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uoucsmsd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3scvuudqx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lpmvpnvy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zvccjflu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ljddqjbv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xtqhinvl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oroeojcu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgfunvif.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aepsharb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyfltv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oqvumarl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gvepjqzk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qiyqlizz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bdioviei.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dkbbjgtv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3srlfuupi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xsqyirgv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrskbeum.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtfrmlxl.html


<!-- 参考信息 -->