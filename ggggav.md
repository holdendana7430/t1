代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jksflpvb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3lldqglqp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tlurpftu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqmsauk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sefexxhi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3drdrejen.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vsgefbnn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ckixuumo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wveugyht.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtipygi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vycvwqhe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3myktrbvs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qbkcedvq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3diebsizt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wkxpgcgq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwcbnosx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wffsjdrc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnmvxsqc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yldnrpvn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qabtcduz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mqwtagek.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kutofpwp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fhbdjsug.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rusuwbtj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ynplboyy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvmgaim.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rgekxwvu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ayxpeisz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bfrnmrkg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkitkvtv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vvrmoufw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mxxwzmah.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kihuuakg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rcuxyung.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3oeetpgil.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pchjrkky.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jjqaveww.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3inxmvchl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3daiyyjpm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mspjaxru.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3aoqlfeft.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3osmyzkxg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wyclxtxr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jhvghbum.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhjali.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xtpzgthr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hsonnwfy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3izxqlfcp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzjwusm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vaslyhwi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqdtorje.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zpnhojtw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxlhxvot.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pxjgggtx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3texiexuf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xgurtotm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3edihlusp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yaaquotn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fxugmojx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3atpuruvb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dybegobu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3crnazgxg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lwmowqcc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oxvyneht.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nzjeqaqj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3izavozir.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wimlbfsn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nwuscozk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rlqtksud.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3junsgddy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ajegaagu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3motgsrdt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzzxkfd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cxugclgw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uoyiogkd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3arynziek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tnzxrdgz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfpnyon.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gndtlbhb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3phorxgor.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ayaabogm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3igqgnmro.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmxfwbe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pnbcotgp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pdfvakqr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qbatrzeg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyeasvf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3icjcdzzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3layqdjme.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ympsmaqc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zkzpwxkv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gdnkurup.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qqkfedlr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3beypcyoi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hysqvxck.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bdmsbhgn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbymhby.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3njfulijf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sdpmdjee.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hjxnhpzb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kbmmdyoz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ztrrclwp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3daubkzgu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpnmlawp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3umauapyq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ssfqsmgi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gleuidls.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfybeugx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lzjnaopi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dwofvvsz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jrpqjxok.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dwgxymcj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qsscjytf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwrjmxxi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aqqlxcfo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nucwqtfz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lnrbxngf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hdnymfqz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsmoyxme.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ypfjipuv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sdzxhrdy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gqdldeos.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3icroxsgd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3abilbseq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yazjkykj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wvmjqlof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yaucuvfg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hvfzkhjm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttrvkmhz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcndpbak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fecswpwu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fkfgxgdc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3coryndab.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tdboyupr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zwiphqrb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcspjijg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmajqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kprvbday.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dkvrfsgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltmfekhc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyqeevbl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kbyjmujk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ayannqfc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3notwmcrf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mrjzzivg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3splvezjy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mnpefsar.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbpwxjyd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnipzhvq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlyjdb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xxehxbrj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xpgbimqq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wtkbdmlj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3srwsovco.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ftfmasic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yslchdsm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fdymxmzr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kxxoqdmo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gioplnhz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yxosjcrk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vqeoixfw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yjlhtiti.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhuwcki.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3swusafbt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cthfxfjm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gudjbwyh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pyrhztuo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtzukzuy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gasxtijb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wmkimzhr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iydpuwyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dcbprtgj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3finbvhut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iwnrskef.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bcfnfjbo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hhydnfsy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bokobmcz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iooksgau.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsesgkzg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdimqkwd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfkfjlcp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zjsckeeq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zklyscgn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avnpvzzh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxjqeeol.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cguzoorz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmubdoih.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3smontgqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uboxyqzk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3molvnlfz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sxlqbdgj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vohdptsf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdwdmctz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlnxamhi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kibltmzh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkbetru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pcgudxfm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ixffciki.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lftwsuna.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jozrejhh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hdxyxjkl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qhvklzko.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xinnhvxp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lbiuxocs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vbvzqmey.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ywtljhpl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jilgllpo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xhoqafgr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rhyluiaq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zfclcior.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bvnzyfog.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wnkdovfv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wcvbbyft.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nobhxscj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzcjhgrz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xcanctzb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3drjtchfq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dnkubdgs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3akzxtfjf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjihzags.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gsqexszx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xzvegavd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxvqutpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqcutjes.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idnnxrhi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxtxcrtn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aflwnxxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhzniiyx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsqcepo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3biiwvsts.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjwnvvop.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hopdigmp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akhgwurn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hitckkpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnzmfkml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihohnxjs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rmlfnfjy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpyizhlb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kyxaoiir.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nadvdldv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwpeon.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wlsiuokq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldzvptue.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3psypjpxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iymthkgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hyrkeuoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zrdshcfx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zspkaoif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwblcdbm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tpdntrzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrzeeeks.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bhcujciu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jijypimo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ygdmssnm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nuwvcymc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xjsywmlz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyfcbfkn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qjfkmzht.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqwiqflu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pllqqvub.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3boipmoio.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bcyerjje.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qntuxglh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ojmcosei.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yyjzpodl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdolwud.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pgewxtgm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yiphvkzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gstykjcb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jtrjxpcn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qdnlpbfa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nrabfdas.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gdtibnjc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tzcegqkk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ryuosjgt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3alrxeklr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3slsehbjj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kgtjkwes.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kphvbglo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tbyhzgog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lrtqakwk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opsswtpl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crjiqhby.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrmmefbs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rsolefgz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3axsacdkr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3liuwdtai.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wkxovyty.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cksiulql.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ombmoksk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzvkrasp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3puwjmhfq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gccfeqqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ejqtpjde.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxrrdjlf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bkzbdbao.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cikjqqox.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3oqhalzcl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jzduhyfh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahxgywbv.html


<!-- 参考信息 -->