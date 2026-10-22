代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cgqvyoqh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ockmrsrw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xazzxcti.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pxdjwqxl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lvsadued.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hmlttfjx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwumqnyi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmggnso.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pryusqjm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2syfxgydt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nctejajz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fbavltgf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zvlegwhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxypij.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cbjuwjxw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yilvqjhf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yevpiusw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qbaqaesy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ieairfgw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2honahuam.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cgknlovu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xxpbxdoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2beoygyax.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dvetqyqq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vqkuauol.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhxitwbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bijuefif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2znaiehcg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmjlkg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkplmxbu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nnotymhp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmwkspu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2thtuscok.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fzfbavfg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vewyokka.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kjirqzrd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gfqxrbnt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fjaltbuy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rupzqaxn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rftyezua.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xgjevxgz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcmfxxnv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjxjhzud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rlixuiig.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrtufph.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2usbhkzoj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jrznldbn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lymrgcdc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mplunvfv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2klizfjhd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kublxwzp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iorofyrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2taqthrfn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2teksobxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmovbou.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skicwgfi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vrfoidpa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2whoqhjlr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmnainxw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2icphdfem.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbcwkwv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rhadkwgq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nzwxrzxx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2atmmcspp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hylxvemt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2amvnbqfv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpqkfgca.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkobprnj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uradfegy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2doofmkos.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bfnccikg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wbkxztvj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2scizrpwv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jbfyovep.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ksahktud.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cvkhgxla.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yrrfwctk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2artxnxit.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hyhsqeof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nsnhupfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vkjyarat.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vnkftpul.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wnudeyhm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bbzbovrh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wrpusyvv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngcfotrn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuliquyc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhbmtmzv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mzwipvtu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2twjgkyac.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nevknxbt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nqkivxvb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jwfuvdea.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lxghiunp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sgyovglu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vzjsctke.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ruqysbky.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oaqvbpdt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqddlnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nneqfkfk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tdujcmii.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xbxgiaqn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zisyywll.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wtrefrel.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jcamsbzf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tbwreobo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cveixuzg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cihwpzna.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cbjhcwtr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2newvtlwe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cttxzojh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2aeftbhnh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2atygmzyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hivpqyrq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2whnazbvn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zezgvvqt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2enmnzcrn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmdtvw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhdemnan.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fsxcrwkj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gaydidmz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2swetavim.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwcfwnxu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hrejdrmz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jmgrzzom.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2trwzlmup.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gbvddshu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tlkynlum.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgdnvmgy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgnnfasz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2naihsaoo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pfzgxapw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ngrsprnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gdtrmalq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2orbmjzry.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rpeznalx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hsdybzhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcniiucc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ruiiqmmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpddksyn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rgqatocn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mcesqnxi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wlxymnur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ictwbsuw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wjiohype.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bkovocim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2okzzoxkk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvaowtsa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjjrqmqr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lstjcxoq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2misxelbc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqesbkdt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxfadona.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gioezyhz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2npnkbadr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxuyqmr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fzcbskms.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hauoqgrz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cjemtqcf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zwwcjdta.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cbgxubqw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hsmbmuqf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2srmqczro.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2awclpbqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yryqrpgy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hoxpdxgb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ecqqqhxf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubmnitnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mwnixqkl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2luiojbfo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmmdzep.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2feuwpxyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2swmplres.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2snieyqne.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2obvienkt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tsctowgu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frxbdwbp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mxwadhsa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufjjigdk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yknajebe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xejfyieb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tzpkkhvo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2sluwdxlp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upxhlzmu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2poxauyjo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jumuaofb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycpufprf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkiviefm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohuimcun.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzljltuh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qkmdagcu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhnbgmut.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtxejzpu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zcosmdyc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tkeyumds.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwzhjtxg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tfykubjf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vzrxmkon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pkldfuqa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2clxqrzxh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xrhacudh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oganmrwe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lvtxqlfl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ihwmsjqb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xmomhedb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzeqlul.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ksldftdl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uitiqyfi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2suqiqssy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2abkrwdjd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtkpyqp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dlutvsat.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2odmofibn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkhoqpua.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nenpptus.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nziqoxfb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qinlnary.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2svtdspon.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bdhnaqip.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2romogifw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kfumwixj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tphrghyk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnrsiivp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lhenclef.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmnjjmoa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbbcdyup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jsxhptao.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvgvnkxq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zadajwkg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqojleks.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rwwwxnuq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxtjukru.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pihkbpcl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfiqdhxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kajjplax.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oatlczdl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cxzrevqw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctizhzst.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kmsyraiy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjflviww.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dauegstq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fafaziad.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ryalmovh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rlpczuqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ycbwzvex.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ndbqbkps.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bmjiprzj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2roqhxjin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkmnsqsv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jksdhmto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgdhopre.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vxvtqdzc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zbvirjyt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zhsziisv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tsphlfpe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2duaeiths.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrdtridt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pexnblqj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2punwsunt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jhhkkika.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2djyzfpre.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fuwiwygu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2njyymxal.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vumfuidf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ojogcdrx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjbkanvg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qozcypmk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2soimndjf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmmcapr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wqnvqbgh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zuxzavvh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fzmkapaa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gayfwyrm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2raouespt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2idrptakf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qbuuipxo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvufhllu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2upishmmj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yciqessz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jrrxmhap.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebuefoom.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zkvndclt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iillvvwc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aybjtilh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mtnrvyrp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wxaolwcm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2evnscwqi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bemooxor.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wcvbrkeh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2odepghqw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iynquzol.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmjoyygi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkfvavhe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qwohasof.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fatldeqv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gzhmmbsq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tviscvxx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2oqlyhblx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yyjzszxo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dckqybss.html


<!-- 参考信息 -->