代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3chasbpwj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sguowpkn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zjuydryq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ypelrauy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gayjdsoi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aqknsvdc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kailfhfx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3otlyxclg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ivxfzsmf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nwpbcocv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhntziu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zfagkbcp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucbuwevq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fhzljjng.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zmhkzsvw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mekdkqwr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3egzjcbhh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sdelexof.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xxjhnnca.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ullbwwbq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ufhpptef.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3reruymvd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zrwtmokd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wxrgwubn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgqmycd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrsyubq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qpiyhema.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vohmppfd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3uirunyrm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soszrfka.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xasukmgm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tdavarin.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uyxpkffz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lkwamrsr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dsvpkali.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ywcevvnu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uivpnkjt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3txdbjaeu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hhrmuqnb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojncsppo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fxrpfqmt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zemcacmw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwodpkey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ngjmkwtk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ymrzshht.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jknupsel.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hgerisgq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ptwptdzn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3osmsbcea.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yugofhif.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlvupcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iwrttitj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcyeyhxa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thevecce.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wwyytxxv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhahwlzr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vppkgotg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zevgzopy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tycbkunr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dvdypyhm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xgpbtczg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3okckmifg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zmdnyafu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bjpcltij.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvifppr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vxonemew.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tckxywup.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tociafkl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeoivhv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3srbotxkj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yruyitia.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oolwuexp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mwvlgirf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niaumvns.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ojtrwomd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3siqqbymq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3japkctiw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3leatyxhv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3twpzpduj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3afnwzqtl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3guxhtkkq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3idevgujz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bckvbwro.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rpibnuck.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kpbnfsja.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tlysyhbb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cehacncw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltyqsabq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxcwksj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3epywocja.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mxjoxfgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ogrqficz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dtqutepp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ncfqgtze.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hwxqyukm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kbrrdmcz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzbjrdy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yumocvts.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnjjjo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pmehugla.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bhpxicva.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pyykepgz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ghfwwirz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lufadmrn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkkatwf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hhoiipja.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pmbonucn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wiuveubj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3himsmmhc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hoctpohx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wytqnowq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mxvtqzbs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hxxqeyos.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ghmznuxf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hkpwrzvw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uwdmhwhd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3tljzskfh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3azggdvob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzwovknq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3svwruyoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3antcieas.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmorqixh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vuudulew.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eetqrtql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3exyrevef.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tpukhmsd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wbuhtqvr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mijniqca.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kjdyhuww.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ifjhixpl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xligoorx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tjqgttce.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uoyzjdbr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zwhampux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3axfalznu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aedvrtnb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tdkayayo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyyonfph.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uzgmxqqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekyormxb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cbermyom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ekumkbnq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ynpivack.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3umpnpetw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mvxdiosl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tazvcssc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3uzbhqpwc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oichwtvu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qkemuqyb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iejnkmog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zxolyruu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zuzykzlk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbmprplc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apnpcrzj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyeihno.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mchinqlr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3utpgyksv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqklgck.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pyuboqzs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zthswfsb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pruesdsi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vhgzougo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpzsuwpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pnjriien.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhrlkgp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hpjbpvce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jvfxqvtg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jgifbutq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zeyqssov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3voufqbna.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qjajjnqb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hlqfpqah.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wccdsucr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nnurrivn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xscsigoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ccolwhzu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gonjvvxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cvcymjvc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtxeyizt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufbzhfyx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrxkzvvi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxxmuctp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zirbczdc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gswfgukd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmrmueqc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzzmbwbj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gpjyckow.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trsutzul.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntrwndcn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etgltkvr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rahlknhh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrxosnpl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgoztgsi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pvxrpioz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ungynbhq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nsnbeftg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3peitfopi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sqvmrdot.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3chsidekj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3nchxqmvb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fljylcca.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hjojqdza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ccfsezip.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sldjjmnk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwyxvbiz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlgidvdn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bvhkxren.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hdrmjjqb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lwgunrck.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fhrdqtth.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3deibuhvm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iuprfpjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ywnlyffc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tknvyvwn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uqeyqvur.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gybuoiji.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nvbqsudu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3txjsoybn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lhtjqrnm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fflteksm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yjdxkdku.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xazccstv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubcjmzhe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhbspycn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmhqfkv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpedrbac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zwrnmart.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whwuspbo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwvewwtf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvqopabe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3brwzvnag.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czmdswwq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvlifkuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnnoujeu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhjfcqha.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aewsoiys.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wckoppas.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuqzsntu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mgxrvguu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hbkylgin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3oixfxowu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3clefpskr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lezotbxj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3usvlvyzi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3flpbvuby.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rjpvgzkr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3klihzakj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zfgwqkcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocknbgsf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vkivnxeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcwjtwcu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qsgfdsad.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lvovgmxk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kbbydzxw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbugoeww.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yjxskdps.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvximlhf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3irpfpvlr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3slfcsdwt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3onvsgxpb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3stkyftwq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xntkohhd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tpqbrjef.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mvdxryjk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbqffaub.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqbihfjg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhjrdct.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cguoyvqn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lmggkvgo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nukzsbdl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vmbtbbjz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3icfnykay.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bxrnltbu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ihltzrbo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3opyvbibk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hfkkxuur.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sxnuyojk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ymuwcwqq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ncrtqaig.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3izveotey.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjfftff.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xdwcqodg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfgcxddu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azjdvzwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqqrlpat.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tnpywnsj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qhwgnwoc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3knuvflsa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qzenhjbs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iklhblig.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3unbtkaix.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lnmxophj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zlcudvmn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wffgrlfu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xqtfwcrp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3siglgwke.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pkjgwtpc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xccnvxxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uicjugjc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xkjikcld.html


<!-- 参考信息 -->