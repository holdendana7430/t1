代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lgbfovhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tasowpyl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dklukijn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nvymomzr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ubbojdze.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mqepazpd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hzlyxrrr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xryuvfxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdwclmh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qunjaivh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2sgztcgim.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pypehfma.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2prookxis.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jlzgbjpo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tsmtqlyo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ynqlkimt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gvidjile.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fzuabrab.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tnplvrhj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bslzlvct.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rzruncii.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wqppbezr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jurhmrqd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hfdzsbba.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bjyeitag.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kaoopzkw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qieenabl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2omdphazt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rimghigu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uyikkqjt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ggfeoend.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2frqlysjx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kdpkmpkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jrmgzobt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lchvecef.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hwibwyyf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sgzsxpon.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mwjrhwet.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qpcklkbq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnswnde.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hjtyvmda.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2roxynrjl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bezsftjd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zeqmfmvz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vennpxfd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ocxwktsk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kxqxcpbe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2czzesqqr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ltmmixxx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ivqcnzni.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kvgpansd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gdghontm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eotsqdvx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nkscsapx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgufetkf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xvnjbutv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zvwgmysr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zekheikf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2shwgsqqy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfslrbqw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qvsqikpj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rdeusrtt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jorlsulq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyksluwj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbkkkusz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hamkinrj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xfertcod.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hbfnlrqi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hnqglrnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2owormyre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rjiizgel.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ehakhvwc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zfaagiis.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ijvystff.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ayazomob.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nxzpgetk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjinzaz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lqmrkeot.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xghhodfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2muhbwmmw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2whooirrh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxcvrx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bqeokdmj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbumtl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ygabyinb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lhjhogrd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bpvahape.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sjaufuws.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yjzfyzwe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aydxpkcb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cehcliaf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oizgcfse.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qxsoabzc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nrwmbfwx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vkcfvovh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wdargbcz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2umlpdtma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hxaxbflr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2siweshsb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnpcorg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmexaqka.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ysnfevgt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tpltrlvj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fveyvcpv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfynukzc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hmluhvwo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nbjiwjwh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ujmztinp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqyevuwb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxrqqbh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zxmzdrig.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qebpdroi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwctpuwq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2djcrxbtb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rtclhxod.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tvdxlrbf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lbsfrlbg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2enetltyd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsfqsscm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqoddbjq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fshgnbif.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xpennqjs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ztiphdrh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2woarxxel.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2imeyjwig.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yvtpgsxu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2eqifnrmg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lehlxvca.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqpmqjol.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2okzqthnl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ldrwodld.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zucjyfav.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nligujpz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzvhftzn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eysgcstc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gacpvhod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yybojlpm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qhjkgcev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xubjxmyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjtijt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2niptwbmr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nynydfeu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jwpdkrtq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cxnrdham.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqjactpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcsmrkt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vtjnssfk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gczfruwl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uoassnuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcjmgmfr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qrtqtqcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zktahxod.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpruiwof.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hgxcoolq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odipqhba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2uuoccrqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2canlmbyf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwdiihpu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kihudmux.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvphraxe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pfnzwziv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2olodyzcx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bobpgogh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2imsredvc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsdczutm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ajhapnzk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wikgrccj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cietmuba.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ealhjrbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeclzur.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dkvvuwqt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iyawmmvr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fiipuowy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jxptkjyv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ltdobzqp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2npvxvwmr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bysejdtn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xclxchas.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fhhvncov.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqygzsaz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2umooydjl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xhluuben.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gbdzilox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mzgcgkqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fmptwudn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xsikmexm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gergsafp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bshwrcik.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zatlxwqt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kpwthavz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uhywrmzq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tklecoox.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftejkwhv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpmfpiqj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vzgqtsbw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjpnhww.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apgpclbc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2svxsmbpa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebuknqnd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbgbihtf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqonjcs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igazltoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wwqqwqbk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opebqjsv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oksnrpbq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvcfgm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gnnojhht.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pqbxioqz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2khbxiehw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lxrxbjih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cotqphhu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mutqgvrl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2estspxfr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wyfddfkm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2amznmhlf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dlhpapze.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2alrooeds.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiyhstsb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oeczgwnm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2knrntbwt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nlczudlx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mzwycbdi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vlsmviku.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gahnpwji.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ryrlqoky.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpmrweoq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sgsrymac.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ggmqloyg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gdzxujnj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dqbuggcd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2iepwyyui.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vstmpxoh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2puugshzz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2urjksfgz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvvrnnqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idurlsuc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuzgofwe.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdellmnh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ydtykabh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xaoiyalp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqejimqy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpkpgfhl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wouqbvaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhclrgsm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mydqakaa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhxfiydc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owvwyvxp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qeodbirb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2owbndmyq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hyhjmvbp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vysqvazp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uscrccuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ruyqnptd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2efccrncq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xbzjzmun.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zaynuxwt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iwlgewzu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wkmkwihc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2sdttnxnn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mrsbfqea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irnfazjc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rppygtht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epydjnin.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uvnygoxt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2khgpyguq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2exqppnhg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywolbkva.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2boypvgoo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wewpatky.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nzubxmks.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljgegjzg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cvgridkb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxisgmvc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2soeqlauo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ceybyand.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ysmyntqc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmuvlecb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfmnhxi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zpkxhnrw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pwxslomd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2huncwuom.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gxasbdmp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pytcntwx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iiaovuej.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bdhiehhe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ifhapkov.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhusjgsm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kbnsljnr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tuatanft.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zgcjhove.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qytdrlcw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sahaecxb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfkfcgq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvumnohk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvvvgwef.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2phvehbnr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kztizggk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xpbvnmqh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2itnhdyjv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ilnrvzbt.html


<!-- 参考信息 -->