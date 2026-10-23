代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wvpsmmwh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bobcczxl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bonynfhl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cytmvorb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ljhlmpsp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nqiqfizx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaexcuhe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3holqvijv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnmlomnh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hvbfwbqh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gmmmogfb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbcpffvh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnlsqtf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3emknrakk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ttvnenwq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrtopxh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dbnkuswi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvoqgid.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rtvsgsfi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pzfwtbns.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kopduzrr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3caslgjzv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3atozzdsu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3scjnbnbq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wrwxacjv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yfuokhaf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrdhnmh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3awehrfts.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgwmfu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3witzhulo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3diyvyqak.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lchtqlro.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rokbpptm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vlzxrvjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bwzeevur.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pqtdihar.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3eagtrukb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ilvcddot.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3eahpkcap.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ghzltstf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mwzrgmed.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cntnduub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prviptly.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ezsnevqe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qwyskear.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ztuwkunn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oubteuyt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xpdygkot.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3efioyffd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gicmevxs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uedkgylg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wmrpivox.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kdaygpua.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cobxpsbw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qhqgstar.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oqxttibh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fcbozjgc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cusoyhed.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnrtvxjd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3grikkagd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tyycxodq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wsvpwykj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3afhfgxyj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lshiuhoj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wdorhmoq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bxosdjmd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bjsutvyw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cjaxylyi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sqpqzsii.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjshsecb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zuabfvnb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xsranwjd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jjdbahxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3olvogpsc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eczkkbtv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xndeutlh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsjxdkp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ounzvqxh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ocsfjyde.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mbhiipwj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xgclpuad.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3sznecsle.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3etfghjna.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sizesosy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmichjd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rjgithse.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3etldibfd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxyfuxb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3syzjcaee.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhmldxk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wqllbkip.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrxbqe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fyqgbuxu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3slyfjfve.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yoozpqpi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3keagzfth.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dvzvvnig.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3oavvwkru.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gojrjkwa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kjkrjbrq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnvdmd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbvjyglx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fwzsryld.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aksmrvcv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vjzmsvcc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tganvroz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wieiznkg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ljemzvtg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yyvdlfzu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3osqpcifv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wqorzhbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cqyfbbfb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gmtlgvep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fpsmalyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ambgidmd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uidzafdd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nisghamb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vfdsthol.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3idsbvpqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zowostgb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3btttcwdb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uykdrlrj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oyliotlr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3utfijzzn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wdtxkxuv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bvmjpoec.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tmbvgvlp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qekfonrt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3slhwdzoi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fozrfmcx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ydmdeinm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dfmchlks.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbwnmecj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3albnlwjo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzheqqyc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ovaraxzr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zasccusk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vidogfmk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vnbbamjw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qymkuoqz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xkhlzyqo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nofolzre.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nosbfdlz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tfyjzaie.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zxnadugs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrqkrbk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qkppbcwt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sralwvsf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eymlbpas.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fzvcjenm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yfixucpl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oncwgtim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3opxnkyfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojdguvwk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3huzrecol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhsigzpp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hjntvkfm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ksorunbx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmiqsqtt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lsoidjhn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hydaszxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mnixaqkx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aklilgys.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frpyztfw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3epmntxwl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qrbrdvxd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3epwepkyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3laccjomz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lrnhqlvb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgxoxfec.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvjoeoz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hskwkuob.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vpguengg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmoseef.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3blkzpoyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dmsnifhe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wwhwbjum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3neysafkh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mbekgekr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ukhailkd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ryohlpjg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yunkpzqm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ntcpdltt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztlsshrf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lzqwbrtw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vqndmhvu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sqcmvidv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gieukvwz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cspxtucv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ndmibsbi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3idkyjkkd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3cmrvrzes.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ezvhlthx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jvhnidrh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mwvhlsoo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbquazme.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmkeobmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjvpurmr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zsebmqgv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqwqzpwf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atyvrsmj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyyemizh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsadhxoq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffjfaneo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcgjmylv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrgmambi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hdgntvxt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqvvwimp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsaydjjq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cokkrbxz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wahpvgnz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3syfywerp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ncpzgpib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mbqbyjwj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxeghsvb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cwcmnwgu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gvcusgdu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kbjyunig.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hvjbxzsh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bmhwhbat.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bpkrqmzs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcpleuz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3liseatan.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qklmnzvr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlpewla.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vcvtbaub.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3itfphyco.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lnxyyeex.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhvpng.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtsimjev.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xymzbnwa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3shzbxkdr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3owoxdyqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zptdfoqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uwdynqlm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aoqcgbpg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3haekeaix.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qneqwtww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlgyvqzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxvxihjp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwweahjt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcpwcbah.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nfxnzlvt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ectreoee.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okpihjfn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdxbrwjp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhqwfbvi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcropukc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3vnnydddl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxahaaph.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxeskdqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ktobhqwf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rhjlqrus.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3izjvfopd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bcbrxlum.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eeevbkgx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ttcnduxa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ucmpmwqi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ctdbkhoa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fomlcqgb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cpynpssg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bywmphrq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gpjvojgo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kihjlmxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wazruevy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cteilgwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lstubozk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sjbxxvks.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ikbuxlkp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmouzoac.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzsdvgaa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ajcyxgkz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bermvbno.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vemfyaee.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ccrrudnu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuygostx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kccjfdoo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kthweozp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lnbrsvfr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgiysue.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrqvtfne.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqifdngk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3srisosdo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gkvjumru.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qyjuohyv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lowyvksu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pxhpgjzm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ppandvau.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3irvpryhp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3aayxbztb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zipmixwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3eiptzhtw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ewxmpvqw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3puuommte.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qtcazavf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jziazmcw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mvhvesbq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nmkgntiu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pabiwlbd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrsruwx.html


<!-- 参考信息 -->