代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xytearsb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzaltxen.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gbslflmb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otnozhty.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfpsvxzf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdmaaqes.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2orqfgsim.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jdkpwgfw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gwgcqyph.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wymnkggo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rzyeiitm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfzwcsas.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbyzwqu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aznzvexu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2oqiwhhxr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2miejajqf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vpfjqddq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tkiestwo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lhyzfuec.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xesjtvjk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gapzbxko.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gaftuyzs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zpglioon.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2txwthwcx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ytjdmedg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2flhdwbca.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bxcsybkl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kbnxbadl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2felxtsxm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lajuwvwx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mroovybz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mlmrdqxv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2korprwzl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvgottac.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tgfvdrzk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcyurlob.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bwbkellp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mvkqjubj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xrufcghq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnjkjl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lvunnswm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iughtrau.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hajgutyp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xppzbrzb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bugsaysa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rdsvxbel.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gjnbcmtc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ikmyutwe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fnuagfuz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2komwxobh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tdtwawwm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yaokpbux.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jhpwskrw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ekfshhro.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xffakmfw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tfyphwak.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rksumyee.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eiggoism.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lxvimshp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ujpsgenx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jvliojnv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ovhbcbku.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2obzzqwvb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zilcfcjx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2szyrukvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rswfxrxd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aqrvrhap.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpxcutmk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bsmyvjda.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jmijomol.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvffmif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ikgdbcfd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gkonjgvl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2quhldwwf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfjvpgsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2efxiddss.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wxvnnrei.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mqilalsi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ncetnagw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aoolhmyv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hwqxbtyc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gxstkqkh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ovacjgcc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lcyllfia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akixbrka.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pzaofrdj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nttooati.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qavtqprc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qtlxrmdc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mawiofrf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ckdcvosp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2prflxilp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fcxafwrc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jzakqnux.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gewwpzmu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2edydfmvz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvgmqhlk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jjbqajul.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cokhvufu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aezdsuja.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kxgjaiib.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ayggfwei.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2afhdegqd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcbfqmqz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obzpbmyk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ndxnlqkp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kqunanob.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bahuorwh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtvmbpyn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pwhodxnv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ydtxywjn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2epnvclcw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2obybueqb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzlzcmv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sbytzqck.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lxnzdbfb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2prcrxste.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tqexahen.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mdoylsdd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmzwuhp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zxfqghlk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gesheriq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhuebaqi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yqvckthk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eouwltsm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2opoxhsxa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ulzixoxj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2eyjqsiaa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dugxpsxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fvfvoxmo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldxwfolp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kqxhfaxp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uexaqrkq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rnctffrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubxtcfqk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bmhexzvf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nkbymvpn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dyokpwfo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qhvgpzej.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cgifvgqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xhtpzehj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qoulahft.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tuigidpk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vowwxdnc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mlgzllkj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qduzkrxf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bvengyod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hyrsulla.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zouzifyh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qsuyiqwu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2litgujny.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dbxjtvnf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pjvhlxrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfalvxrh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qpocyhmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spnzacpr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tsdextuc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2psxpmsit.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcrjepel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xafllzfb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lybujskf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2srrolskf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cyemqnhq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wepyhzdx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sblvxnad.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ffblyxbj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tzzofaqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwebivpt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfhrgbez.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymkypvre.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dktwxtni.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjnwcmj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ymgzjpwz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbhtzeyn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cbnntnan.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ocbxnlwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bssqwrmt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2afezpvnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gvnvcklz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uevhxgkc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxodddq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bmpbrhli.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gblfbgaq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvevmsbe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qatfymkn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gkpjdhto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dnwaqcrk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvopnv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mkbqpszq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vuldbyjf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2lspkoots.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wxgcojul.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rzjbqxmg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2svltzsfu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuknpgtj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbagbzip.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stmklaic.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2czqiapse.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2oulisqph.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjdzpvjj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mophnehb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yaxnblvd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnybziqr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kdjtdfvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcoohfwf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tywzmkao.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cyejlexz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfnkfumz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lncptomn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymtcvbhs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2odgzszdz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hjsvzhaw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qdvdkynm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhvfrn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2azmkfzjc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2coxryhgt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mwyebfbo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2drwldzgi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dnjzdpfa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qhutyiyw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jsiiocuk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rdlwxsvz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2erclhrwb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2evxgdiuo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhfwfyg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zmzwlqvu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wthjloqk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ypajasme.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2shdsossj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcfcpho.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fqctlogm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jpwvtwws.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jxgxnflg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2raufwxek.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jpxpmlph.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iejcdmqj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uhhvzmwb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wjqopcux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2espqrwzg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vqljcnjc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfdlgjeg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gotumfls.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qlmyimol.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flqtwcyg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuchccev.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2badssjlw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrywmutf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrjnmrbp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztngttij.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ualcwvgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oypjvrwl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gkfcftok.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lngrdcyy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqfsdjui.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jvtoaspd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kagkyrma.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxavtui.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2meoriqgh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bmiglabv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jfxndpjg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bgqffwbf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pdhdldgm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lkwhpsae.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rhjmplpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptvetbsx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ujequmqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qijvkadc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eywhyvcc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ehtgimeg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zedjxmii.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ssotgthi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkrmxgg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhszcnth.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eizxcwyi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2thwpqcyi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2avtgsgbq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kqnqzmkq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rcpmvurs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rguonfsv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xagzylxr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuttdflc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2workpwuf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sbgooebk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfljcgbh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrykgvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rmlvhutl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tdyjwiwd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jxvpijvd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpidxcif.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lupmqobi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sviymmms.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2guhzhlbg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xqzunpdp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dlhmezwl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2egaxfobw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wayddouy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plxdvtfi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thlyzpvu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bojitijn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjsbioh.html


<!-- 参考信息 -->