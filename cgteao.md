代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fxftvklp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdysilav.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhmpzptu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hvubawwg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iweknerf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xngblomx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yunmvmha.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rlerojon.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3daygdyit.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3huxlmqkl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ehttraxn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uqtfnkgz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dzzscxwg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tcxctxfk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ktuytsrn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sngylyiu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ylnbrqbd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jmhaauob.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ilvgrncb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3menbepix.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3drkttggr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kyfdekcf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxbsfecf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jufqyikl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eumlwaij.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oytlttcn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pbvwrulu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yutpulam.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmrrptn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdeyfhs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ipfhydet.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ramqndpe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yyqefqcn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qitkyndl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jsnjnxwj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mpngtwvf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xkmkcbct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qmmofnfl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nsvcuugl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3alcvvshe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cuqdhoam.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wqsxzwyy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fxolhqyp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jszscyyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vcdnekuh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nmjneyfo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hlpcqyrd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hevufljp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3faubgjwv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmhbavc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3homhcvxy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xyalitqw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xksfdwsi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3appamurt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pxixhgfh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zvjvrrou.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ytgopprx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvbazjuj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ffzywgzc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hbypuhde.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3iohqecnr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cazvjrgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cmknfueq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iybmefne.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgzpvsm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ufhtmsrb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fthsnmzw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioolhgxz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jxtjpycl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3odxingsr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kafmooof.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3headuqlu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3csigjguq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kkdiggog.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwatuvdy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xqovewph.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtepvocu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3khwgrlay.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3arglxjbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oniavfnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcvkjlw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hqfutmbw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iamsnvcf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovgfeauv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ucovlwgi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qdwpsqve.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3usafbenf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3atkxopnm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3crxhtaqe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tolznmnc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zicoizqg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnbzwhjb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xtanedix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wzfhkdlb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3agovrdrz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gjuubnev.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tomkilqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3trwflics.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cgfnbakv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3sazplacq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gfqpovga.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmuhjwth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qsmbxrzf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvtiyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rulmucxl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fhynfueg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zlswjvsz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ihqkdqvc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhyqucxk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nrasrwrr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3loslaeou.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpraiwyh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3auxygdci.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ufatplgn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhszekub.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aplcovvt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bnhhzyuc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vsfhzpwo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fxpcudxg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3epkwammm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vcpevonq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nercxmix.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnpvcdda.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ekwjvplb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ehllkxns.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wvdaschm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3usazwdxq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ueaiewnk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbjgek.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jllercnv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jwupcmnu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lwkjsdnj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jctoczys.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3urppgfea.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnhicuww.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lqqarytm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zdlyusfr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3thvmjooy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wbrqhguf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rycndyel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixojhafa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bluibdqb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rtqmexnf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hqhnexox.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nfgxpwnw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xednnafm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jxwgqvyb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ltjoaqlm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vabsmkcz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3galxfjea.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jnxobolt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvzqfnop.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ddlmqhmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygapajey.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ubdkzjfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxbkygal.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrohhaku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bcuoqiic.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sbykiney.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ywehetfm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vruvlvrr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uiiunhgy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rfupozkn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdkuksvo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ikefxtap.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cawmpycw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gddnyvhl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjswtqei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnechqlv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vaueveei.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sazqsxgx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxaknkx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3msckevrw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ngwzumds.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ieiieccm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ssiestpd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pgjbqxzq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jprcvxht.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bgtitsbq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rwhenvge.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qantutky.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vkgvjkfd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kobbwtly.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvfjmovt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ozeovufw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sfdlfqly.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kwplywmh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3forhzjkg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3eddtchkj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hohkpitq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yxxhmlag.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3psclwvtn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycineebm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ecdyfnsy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jersbwii.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrqplmkp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwbnbfkz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3euuhsdta.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pamdrvrl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpxedspk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmlszjdg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ktwkrhvg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnddzksp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmtljduj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ignodtdv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvwiqeio.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cfzthpvn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhkxclns.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3migfwmdq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwpgfcnp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qzbfzvnq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zsafxaek.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xytfntra.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nzojrqtc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dwgkqlbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhimjpwd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ezzffjgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3crjigmys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qhztwxax.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3crggtpbo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ltpbdqcl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxwpkjft.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3viwhkton.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ysthefod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdgyumm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nkhyaaak.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kcchcncv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hvcoxpjo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rixafrfg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nixnxush.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iehgsxpm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3clxyaxoo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tgotzqns.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhjbdrlc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3otqhbptk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nijrnldt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3brhgmgqo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3oraoassj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjjinksw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcwknvil.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gguexpbm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxfldpnp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zpypkpsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxfxlxns.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbvxtyvl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyklifuu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmodurvh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwhwphlp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3htkncpyw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3soytsyrk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnaiifys.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qhnmtkcb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rnfofzqo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3apzzdegl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jwhqdjkk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eycsmzpt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3izieafqh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wjzpxabh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3sdrpaygq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rhigftkp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ilrnbfip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ikfkipdj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jdctmbwx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xcuiqonq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqlzlwrs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jtxjsyoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpoubmyg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tkjvzvfq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ayjzywdv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwcgzmhu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvmblkdl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hqurnywc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omqfgtee.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gwymtoio.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vwmtlmzk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqowifna.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3naeusxsa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bibkpqmj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eahadmup.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdqszzdv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fmvjzufb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3phsgplru.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qtkfcytg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fcchssoy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xoavwxhv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zujlfdaq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sclpbhdd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tnzerxoo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3urzbwjzs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wiwkqsfq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kunhggkv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rzlaesuz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cebidnuq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cfmtwiom.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ygdvwwog.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3huzjlxfm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qngooukz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grqeshwl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkukaalo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hnxdqvyk.html


<!-- 参考信息 -->