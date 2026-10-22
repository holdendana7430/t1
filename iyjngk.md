代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fzgtfmko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrvhdptw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2phvowotz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkzmea.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmvzitwd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozdttbyo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dinaixdm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2laxrhplc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzbjxbzd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rtkibawp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nmbvwcfz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zfvfqgsc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmcjtxc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nbatyqhr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2waqhtlzy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jdfwhvwl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hpxcltkt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iwiignqz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hsjxorak.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2earpndpg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xgjxexku.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ezsnjxzf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iyouxylc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxcolxn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2svvutofu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sxaenkng.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kcavfqnx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tgobqazd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfgsngf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnuqdjwh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zluaersy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwchpdbe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2openduwl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2iodhobma.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tqxaeemf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vxquhsck.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pjiwsfnx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2smebbuuk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ltudvwzi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ebeuujel.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2brxjlqdb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pxeelsmy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pijnsier.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fovrwlkf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jdjpjaya.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kilzpudx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2myzjoxru.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhqahkk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ulrufxdx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2posvlcpk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2oirieiss.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dqdzfksu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lghlrbrp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xruphefe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zrvgxtna.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jjuwszgv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lortpgqp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2afzwxotg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2glymcytx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ekqhjlrj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gnwhurqo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mxsgidrc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2muiwbcgs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iqvoouql.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2snfaqzdj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrckiea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqpksip.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2picfuhey.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixahblll.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xixmuppi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qgaycgck.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2couvkkba.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yvshipdb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kvsdgnqd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgdxshv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yexuhfvl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldocasuc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rvggiivn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kohvourm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrapsxfn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xvhvcghi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tdvqliqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kstnwmgr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wquxnbmh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkapqjcj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hyrxutbm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rgcufcad.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pwavbkls.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdiithr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2esqvgufb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ekaeoztj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uorivfjg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2voyjfofx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gqzpolrf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zffnspqg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ktagxddh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xadmyicf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fhmrhmlt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cuwabtth.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lqbgybgk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2stvqvudt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndarxpcc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkkvker.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2riujvtbf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyeqhagn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nultdxcm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jeyahvoy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wkcmnmjb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cctazxoj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tbnmycvc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2llohizmr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2haafxonx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gitamukc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vouapyzd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dyitqpot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pfoialel.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hgfkellj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gkhbztlk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2velrgelk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hemsqqmj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxkwhz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pedqrcyl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsrxzdaa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wedggptk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ysupuavr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hakjmthl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cwzpffhl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ytabkgwh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zidqzgxz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxofmsea.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2botakmht.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zysrvuix.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jhmsmwpu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2swbateow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yugwylmf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wukzzulj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jijrbail.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ipwejspl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bculialn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xdiqhfyb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oyxvmggf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rseaprwu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ynbbslws.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mhnjowgh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ilsrqoqq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpdjyvq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tvqprgfs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2andxuvac.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fsnazufu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nwjsbffi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2undyeyrv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rmqnnaov.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sbuhzolt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzlqhroo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vvjyscrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tinnmrpa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ftckskmm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yapfdvso.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uqcwoyll.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rasvxrlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2okpggdcn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cjebotdj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jtycuthp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdyilofo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgypgzyu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfusluby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2glfbtazy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pgnexylm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dbccdjwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plfervvk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ncngpnyu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpegcjuh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bibepvri.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciskazrp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ljsblzmn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wimxrozl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jjtpzqkn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzutxd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rniyxqhn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2acvsxsel.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kdkvohxc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kjpjeelw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlensx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cochmhhd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cjjfwbet.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vldmtrtx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qdwigerd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sssrkgzm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vqtgickj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lipjmjjs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ximhemau.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ztqriytv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rqzebaah.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2pgvzllrv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfndtcgq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uabazyds.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euvvicxi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qnxoyqws.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wqgrxery.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvvnuamq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxncbirx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kqffluur.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctvjzdsk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xjbhhpzw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cysqcicv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmlzmezt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lttosyok.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlyvrox.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzvhlsso.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hpckzeup.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2drtibryz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vwhylkwe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mprpufcd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2snalfjlx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tsdyhfin.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xdalqmcz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2prhrfguv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xubzdeqj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ajutmrlp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xaostzke.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hnwoiall.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbyecqec.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ruijghtk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwbagkqw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pufuahnt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bevqhmmg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2beqmydef.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ozhzvlpu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gvmymtfj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cviuslsx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tqeaxhsl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2unzznpih.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2usmtbpiu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2copjroso.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pvfkxaal.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twhlosan.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2whnmlita.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jvqqjyme.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2camaitlz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixcahntr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euzeniwv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfjdtgrv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ncwvvooy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awgutyoa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfhtukgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plnfjltt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvhpzrgt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zynwoava.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wichtbrs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkbrdqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dufhvcff.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmowgakj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mumjddog.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjqbsglk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lyqupdfw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ndtgnrgy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2eamkeotx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zqyciqtg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lpuiynsa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jsdfzahr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dtotdvcy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bsifazia.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ibiiebyx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rrjuafbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqfdfjio.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wbjobjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cezcifdn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xxlmigct.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vsgolzpx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rssoxfyx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnzemlyk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2exdtbgwv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wybysrqc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bnmlfujz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wnnppvqd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wexsrtdd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvzterpo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2evdirvqu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwfgqwob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsuygdf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjadiuku.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzoldwmi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bhxszxku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2roysdgfn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eogifbwl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pibdhxxc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vfolybha.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fkiduume.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rlgyjwnk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ukopelns.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2irajxhyf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ipjfnqaf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cbvzkgxr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2chplsypr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ozmgwblk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lqwmzvvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbzcdhld.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbypkop.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rssguhax.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kdgmkxmp.html


<!-- 参考信息 -->