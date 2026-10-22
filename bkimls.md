代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dntboyas.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qdptnuke.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zipwnoyy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kbxvuspz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hijxdmcp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwcberqk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jqprxpij.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oylrraut.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mygcmcqd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nmadlxdl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2liibnvig.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hoenobba.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hbsntlaq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2leokzhwa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tyulxgam.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxawixl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2okctrtry.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bractpsh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uuneskgx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oalaieoa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zpunbtcf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyroskao.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sydzpooq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vdqndkzo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpdnrjur.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hcfvyuch.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sbtabsia.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mkyaxjmj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tsirglmw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ichgzowm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vetzecel.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xnwhbijq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cqzerrzb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnrcofa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xlvulfwg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfydvaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2olbgobgv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ddgmemgl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vistvhnc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnazqxqd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cruyhgjk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgazgykw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxhojzmv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zriiqtxu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bgiozcjx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gdcjlqvo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mltljozn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ppyoigbv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ufioglam.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjdkayeh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctcgyscy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ogbfezpt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pafcshno.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2msratqqp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dghwmiaa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xyhsided.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2eyjmpldz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgbawai.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbxkpnl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dzxvdzsa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ppcmbcbt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hlxgsqsb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hwerzshy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktonvbwa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bvdrubiw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2btqbmria.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfcuhhco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bhkpyweo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lctrdubs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qiismfvz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2splirltu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkbpzvl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dmukxtbh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qnjswujv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uircrrte.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lfktntru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ybhvkcea.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lhajqblc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cesuihej.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mnjezssm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nidiepvn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jtzpdiva.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wyrcxjhi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2orpfuhmp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2nnuukrmg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rjhuydjl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nllasqkm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wsddmtfr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kkvmfffe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vdxsholc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nfqwensn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ubqijyhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rdtjhfjj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2larcynlu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pbcfwoyx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbqcdms.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zebczgpf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2froepinl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dsgjtwdy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2khjlnpiy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tclapxor.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gwpeznfs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sehtiegb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vqlbcnpe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lnytsgda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fcejqydl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2otmxxoyo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vylbxnad.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pxozcqyh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vtjqyghh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jgcygjpm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvobprvl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ashgchca.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jjvvrfju.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2klpsymxg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wjyrhxdp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wzxxnwum.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wfrncncc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gaedtiiw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zlfafgzj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2chvglrie.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vsjgplui.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hnnwqnpv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sivkvpbl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2avpwojia.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xiwxulpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vxhqptmq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2koqwaaxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yrdmzsah.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pqwdswuh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eldeiveq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jssmvnzo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kpduqutx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2padgfjxf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vhunobup.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2otpbibgt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qejidzsy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ymmchzkh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2glbieher.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2voyxewul.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lbwgxrga.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yqddvfph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vvywzkco.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wxcpngvl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2oncrgqoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfifjszo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ymducuax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttgeicat.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ebcpodgy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xjmdqbyi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uwffrgdd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2brfcefyd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cgcyweiy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngnlojwk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kinihhdy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwlqzfkm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swscojib.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjoujkjq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2evfgyjmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbygwgzm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bnlgxadh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bogtavxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtalapt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynstfxul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jezxvave.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsiqrnxk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jyyenxht.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tufxznwj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fgfbeiqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2okuduyze.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ciageahm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fqfvjzgm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yqoqoqbg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2puzhwvtq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hqfjakyw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wfagsqlq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vltduzvn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zgtoirop.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qvbwqosh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwkwipsz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmqbhpw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ogzfzavu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kyuffxzl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sinnxnbh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qnsmdfph.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ixddvswz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dssisrqs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajbannuf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvekkpiq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2whnlbced.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qthrhbod.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yahjyiei.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmbpivii.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dxeneikj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksyifpaf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgrhmtun.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxrywbay.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryenuuba.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrydpwda.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jayfodlm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irorycsg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eekcqigo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gagabfbl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jngxxanu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2htzmqqxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tmuvzyzo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wskqfhdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sprsluhs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sorlcurs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rtojfgop.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2oeqawcqo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2velpdzch.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogarxicu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvwhoizw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hzlvvpbg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iwossrvi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vlaoliqu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tkhceyso.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kevatdyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dtpxadht.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vquuvumw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hklxnaxo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjodtkrd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2edqjifti.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tgszdkle.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zhvywira.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2iwymohwa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djjtakgd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2agidaltu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mziqkklc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqqukhj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzkxrumb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkjulxhg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndnkwdpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ntornnqj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khvquvog.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhhrmmdk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugwxoqnr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnwutqzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxnaogcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vljszequ.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbopwbim.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uikiuqnk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2chubnasj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fptiibtm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trdgulwb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rwzzjsds.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pwdfxkrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzaqarl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bwjtfunt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zojxvjzz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cdkzgzgg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2taccrlsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jqvtfcdh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lntliflp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2igxoirab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hicobshl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ofcgtacv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hknmwaqe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vhffthin.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vailodhe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvpoxvjv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2omusmbez.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzltkpzf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vudizmmf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cklhnsih.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2abmqsbwk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yoesukxx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvwuqzvb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lakwhfdx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2airfamoj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oyawksfn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2oyhtffiv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnorvguj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pmyaprif.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fncyglsn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2etjkjznf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vgvozavm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hstygbdz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qxkhohlg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xnebokdp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zgdamowg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2avvramug.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cvfmnvvl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vqoyqsqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nadyckko.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kspqfmxd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zevokerb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdggxltm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfyqnixk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jbsfdnoe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2netddjeg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mmnicjmu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wxiykxmz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qosgzfwl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jrrvinze.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xvznkmyz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmekxnys.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oaytxsvf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yiyuyxlk.html


<!-- 参考信息 -->