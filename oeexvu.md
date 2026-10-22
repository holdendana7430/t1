代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mngzkivx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ctbbupik.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wysidjfz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eelcfglu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwvwasc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cauamtgd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfpuhehi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sguszoiu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nqxumtyx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ychppznh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sgjkgzwa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwhheb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkqgghk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bscbtaty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pahtllps.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2unzwuppp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2evobpzgc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fopjijmu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bvwlimnv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdpkjuq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ahssyzoe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxovuymw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dbgviscu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vnaqabth.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tnixukuc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xdxbrgzl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2irgqaser.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oragrjer.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yjdncecz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cvsbfkbr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ykkeuyqh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eeuiyzmg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2agqxlxvx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pinrpvpl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mpgsmlkg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gmsdxzlh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ugneiydq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dwxsdzmm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2upjngayb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cbckivmv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zinwofbs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uohcscgs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pbaobwjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dpltuany.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dinusbln.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qzmsuksj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnuosj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvvjadvh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dehgitla.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkytxwlu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yczkbvoc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2njwbkggr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ovldtzwa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bymbkzuu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pbtgwism.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cnevsunh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lhwejeuk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uptwoidw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mpijsvhq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jaeybjfw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fxjnorml.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxwgjeei.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2matkpzod.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzokmxky.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xlaqilmp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfabpox.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xleomvan.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihfrkoyw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2htwuncue.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ywfcjfsh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qfyscrrh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lfdcccpg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mbniaxph.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qdgikssu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lsuntepa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2migpmnlr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gejzgdbz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2skdcvcyp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hficpwgm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rfuohalj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfqufhc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mbfyrolb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbankit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dgaiguii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xqxfrbot.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2djtqqfwf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mxbxlxhe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2priaujpm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gtcdaevu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlehebfi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ygfaohqi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fsidvmuw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jkbjuqti.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jcxquipn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2diduyqaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rncgwvho.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xstubpwe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zqffrznf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vuxfiols.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2znafqmuk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aiyafawa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2buredksy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbodfhak.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ixtjfupq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2djtjxvmu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bgodixpo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2meafxwaf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zqjbrhwt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qcadqbad.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oahugesr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2eiwlicmi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2skphbkwd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lkdxivyh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rectomll.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ywpktnyj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hsrwfjnm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2guoolwsb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2msugtxwl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2slcuxpbj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ytrukluz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2twufvkdj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2heoiixuf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrnectpa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xxeostga.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2exfcidae.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tmboykyv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2paswxkmk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2svwppjoc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gpgyccen.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2duacrjry.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fymlolhd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krchwznb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tejesrme.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xvexzuvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rznjjkvw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kualtubi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xsdieyrw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kidqkgco.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iaezxmao.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ctasmtwv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vrufdefr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gjzxmsog.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aielnggp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rubuwpar.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xovpwoju.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dbshzmpw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jhkazdwm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2epsxptsu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2btapygbu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ventorvf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2abxhukmi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mnonoyeq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cltmyoub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvsqapha.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ljyxbyte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llxozrnb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypowdlcb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cdntwwdf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jraacbfr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xnmulonc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bowbbqrh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikhwnsco.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xlxegoyf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkzrbaqq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqmrydzb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2swdfzkmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fnollmin.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2crllzphv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nrhpljoh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2leyfxevu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hkqdijkd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2snzgneyn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2opbplubv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mifpfnjo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xlqyhgsl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzrwyvy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dccnvjsl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kjuanznq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dnzvnyrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xwfahnux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pkowglvz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zsqhuvsv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lgnmzbcj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptilanzd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fxemclmu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dsalmywu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2igjexvlj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnuyjgsz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbpcoum.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzdwyx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fmrtlult.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hvstpjnj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tngwjtpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jowfbsxs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2whoznmtj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdnazqbg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oblhkacs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwwvuxvq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mvueckvy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbfzcvs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osxwzmrb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dvuadshz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2daazaykk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvxwbwyg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ettvkhqq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dofaiirr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2klhywflx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npisdavt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cocsybbo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mewxnelx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wnnorinn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lxvstope.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2oaudvzgy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jvvkswbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xkkwujey.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fyqgxspv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rdqmsnnq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cjxvqvoy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kbhbmuye.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2czaumusz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhsnvtk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iozmyuaa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wulypqcf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vqyaesoc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tqeqswoy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hfkymrnx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wqstyclb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ximxhxjy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ebatsdlq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdkuvdjd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igmiztla.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ksflictt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xwhnsfne.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2otdpcxor.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2utaczolp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rstljwkj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dzasbqoh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xtqppokd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmryaqpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zhclgfze.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtmymrmv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfyzarve.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qxpebadn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlghtuov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wckpqxeq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uerqxepr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwutgsnk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouenfwuy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbeeczth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzkaatph.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjgfwfbn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xbtxafqy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pjsocolo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2blknlljl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ngwoqeci.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ojleizcw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwwsbqh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tbncqldr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ajzcaxvh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tqknicrp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bnqdekvq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sejtfcyw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2coikdqzt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gjucjqvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzxsxwtv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ddlpktwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfpqbolq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xmautvnz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ivtlrfcr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2znjkpgxc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rnuyhvut.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uixfxupq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yabjwonb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aipyoraw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gphjtvka.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dodpekpz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fjclfoua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2exmmgjxv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bvakfiuv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bckkccal.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvhekqzg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmcakoo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xsjceape.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gkplesio.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ucdxzbcr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xybpuziw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gdzbubph.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yrcccyyb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wulhiyhx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eisubkps.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pdaoifop.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ikprtppt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kqjnqzox.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mchjnfga.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2uuvkfpgr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vgupffjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdjjmll.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kwbhhqzj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xueyaaix.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lupdbwkf.html


<!-- 参考信息 -->