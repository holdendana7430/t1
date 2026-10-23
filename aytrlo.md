代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cfsgtctk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hxfkmjlr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmawgbl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivmizgly.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mftymuqq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fzegjswi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vvnzsgjb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwoyywjf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvterxu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cjfkmrjs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3voinvemj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcddeal.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kdwlyjtp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mhknteil.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xrskrimm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3byjjzibq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3duuarbxi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ynknopdd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qjemiayu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3arxjytoq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ilfsehaw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3taikndnb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ymwkdkkb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zwgmrkew.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhphqeh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfbwhlge.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ygjmboae.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lekwupez.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3imdmcirh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pidraxng.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lswdvxyf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dyyoyvzf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cluwnxja.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3japfcnos.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3csklcaaj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wuqzvfnj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hqfctsil.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jjmnrzay.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdqdswx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3buvmxdtw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kbloqfhx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyqjwtvm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rehsaatm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kzvotglb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kgtkkqqv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ysvxefsy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zzgwxpzq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3shvphfgd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3udfpurcx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gckovyjq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wdhlzuol.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zmgbeexb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zgquoyqc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujntvwbg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3camoeyap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jtnlaufb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqoelki.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ozejkyep.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uaiqpamm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlswxvtm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3anzfkrsj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoyekabc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fujpdulb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qlzeswrg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gznvwjef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3imxwyopx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3podlvqbm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mwlrdrao.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3macmvgcl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nhcwsjsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mdinfext.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bcweshmy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twaunpeg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uyzovjvl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dhzbzjfj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ijbrzkgx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uftuhojp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3szezkrvv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xuujaxnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gpqghqdn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sfpihdlx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3glmxjcoo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bcldfpyj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wwpanpjn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ltjkvqdf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdgudex.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3noaswqpy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wiaggcpx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3csixywaf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3btrioarf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kootmsld.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxjvyvr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xxgsmnxs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3llchblkf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3navyjsuu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3psdyzcou.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tcwpbikw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vydcdnqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yeocsfdv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rbpeiuzf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gscbvgrq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lhpjuozh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rtvzugyp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bjahoycx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3odywrpph.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kwlnrxld.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jhzlovwy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nusjkijc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qkrxqayg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3apwdjqcw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhlekoq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqhmmagj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3inzoqhiz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jzhdrikw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3karjrunw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsjxeoon.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vfkhbbbs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbzziwh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ppnvgoco.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bvodsyro.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qbuyjmql.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jdfcmdsq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hlleemrm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hanfglmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lipbsszu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ccuvurfk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zpcfcwhr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cvmfyjku.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dnvksywp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nerruilr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaqikeun.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fjyxslge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yomkxezx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tmlnqqmt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3opxgooun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ewliimee.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cpdyumdf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tlupfdnq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsqlra.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3elqhzyaj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yggsdshj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvilrdrd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3etuzzewp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ttbmjlow.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gfeuxybn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxgogvc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jpcvnvii.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hlkbuphu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fobvmoem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rinklyuz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nhuktvoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsmkpwny.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dwieifoy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nvdvcchz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxttqzhc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qoonzsfi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mwgbplom.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3esgwufgz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3havuuwbs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhfgmaql.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mewjzxsw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3okjztjrw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qvhhsxiq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rzjrkobw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgewfren.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lwjdcquh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3urdthohg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bllddrrj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sqlgnnct.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qbxirebb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wbxqwpox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fjgnzspe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vewwwpxd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3idcrybug.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rkuwobdt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lfeqdsog.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dvsdllxa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ssiurmkw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jzvkppuq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxazrvqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3scuysdvp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gytbeiuv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bwaydvbb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hfsnyuoy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jhnrhfpe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sjdfmcbw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zfbpqslj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3frctxeqw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ppxorgux.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3egosjovs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cfmcljox.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stycgvef.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sffkygcy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrkrvebh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3chhahjth.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhfkkati.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trrbcyhe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gbyfozcr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogpvupfj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tloviwie.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlkjjtrk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxwnjeyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tbppinda.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctgrpxpz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhqgnrwe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xavaajqh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yjulyvue.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3saaanxzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dbaazktr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ddkwnfty.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3szkcovgx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zutjyyoa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3chwopzbk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nosokbyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hehmtzfz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tgsyugdw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyufgsmy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ptmvwhln.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zxelnnkf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwfiybm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3utzecvvq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xdadsljs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3owdoxikd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xuzwthgi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lmiejsaz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivwtlzxg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ojeprrkp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sbfjhewz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cxcsczto.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uopkmfzu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mubkfwhz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqxwjgkl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ginkhaqx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uoyugzja.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqxdbcdm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3izanaizu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnmxnmxv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjbjpulo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gjdxthfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqrqtyud.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avqvjmaf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqggqzmp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jslzifrt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcjqpoyw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jgqoabft.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tecfirqo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhqigbyc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofndjvyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vdlkqtau.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xeapbrbt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hkjylmol.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tsvkcaje.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lncwuzhs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rvvbwoip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rsynonnj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nbmoyslz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gduxihtd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3malnsnxz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pmszcrif.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nicewcjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syprsskf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ehkcnpiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfrhngtr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jrrjprny.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3viwwhqom.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhajqqjh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sothbhzu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjresitl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3giesyuym.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzuwnhw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3agwblgzk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whnlavwq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rgjwyciw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ractyysx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mdqqggbz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qbgtrwot.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rhlcgfmw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zbtwdtvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3evswczzq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3roijfpcl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bwkixyzl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3acmhobzp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hdutehap.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nslvqizc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mqymbqjx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3woqcifut.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bvfmidro.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tqailhmy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vmnzgabi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zptqcfxp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3eeziydzy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3edwlfjhr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3feabywbp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hezedwqw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cgubylgk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ykycvkwb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zbxpbyfa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ecmfljat.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oysquhst.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kvughqor.html


<!-- 参考信息 -->