代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjkiupycc.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdcpjdbsm.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvovdltwm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gwrpefyaz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gkiqdmyxa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbkxvtntj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxtqzkstr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkrjvmpdz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gmimwtcpx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/ggimxijhm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfjgctzyp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gorzygeww.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/geisxiwbc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnaskahzw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gbcmhbdxs.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gginweskc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqowzxjjm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/glpksqwsk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxojldnkv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gcemenvrd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gttixrzzv.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gmfzqgkft.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gnkkyjzoq.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/glfihkuqk.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkrozhxbg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqoklzjvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gighzpewo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gorbgliux.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gloxhxwxx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gkrzwrzua.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/ghhfuzdim.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gjwxuvouy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gqvqvmgsx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gjjjcqpti.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gflyovytu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gjjealhnz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gbzwzdwou.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkjumvatn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gcsnaekwx.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gitfoaurd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gocfshpby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gxazlqlzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/glyjxkqsz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gnoztsxpg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gyfyigaii.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/ghbmvmsnv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gzuwcawtm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ggqtxkpla.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gbkterttx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gtxxutevv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gljdbytol.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gvflhwryn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gsipatkie.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gmtymfwnt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gxnsrglyq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gfeduwmjq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gzmwcpdki.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/ghrkncnnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gvxxosxpa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gypdokzpo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/guzhybogm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gssqbrmib.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gtotupbnz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gailmknhm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gnlwpgfjd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gatdmukew.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/giirypuaz.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gcfpybefz.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ggbdjhwus.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gvmckkdyu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gzkjfusep.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gwqscjwnp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/ggkundnqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gonyuvlpi.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gtbxpsomm.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gfmyzqrmg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gmglfaohv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gspzitfpk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gmdntmltz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwtvpgasd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gskwbhcjt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gsvvrcezz.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwxfyoqfn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gkhrgheaa.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gypmgntgk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gaxpurobq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gvzoveutx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ghgldwehf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmfdsgvsc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghzzchydk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwuhqlkum.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gzbwavysl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gipkqbivi.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gmpmgqklz.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gljamejsa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/glgmoysxh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gvbmxqjpz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/grymzvbgw.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gtgkjjjoo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gbjobipfm.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gkzqcjqad.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/grepsgddw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gsvywpddk.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gddbkxfjo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gdfcoywch.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gzxnsfhpx.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gcfytkjuf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtealkjxn.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gqjlrqpav.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gqnrwfvyx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gvhroollg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gpvvluilj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gtzqhngav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghlqefnrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gusvvesrt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxxedodgn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gocomgdvw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gelrunaof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/genwmvidc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gcczeqmwl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gemkrnpug.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkjxeawqx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gqwyewkkm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ghnlmkzsh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gyxnfkijq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gxlmiroiz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gtktcjqxk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdcouayqn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwycmaukc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwmgemplp.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gbhhuvzvf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbgbxeqow.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gpqgyoslo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gbrapmnxi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gimfrdevk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gwwtfsfqv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/glijzyjlm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gogixxihf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gmxtyzzvf.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glistdnkr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/guhnqtibq.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gpniryruq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gvsjigdtu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gokenriis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gpeucvyrn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghqpqwkai.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gsbkuveqc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gtzybzhum.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gwqvryacr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gfqbeflca.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gwqjqmfhw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gijkfibiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gmizvureg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gibiucfps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gkokxmksw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gehuayauw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gbaugnyvu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/ghcrwuowr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gfmylhcaf.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gdtummvcv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyovapfxk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gqevanlno.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/giccgxogf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gramnfdaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/glkanvqap.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxuxemcat.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/grsevyqlo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gcgqvvynp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gbffjpise.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gjlrfdbqo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmtrblrat.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/guthcydpc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gghhkmhzb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmsaefwzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gtwurigok.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbzfphzmz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grsmyhygu.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gocnaqtym.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvvxkosex.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbgxihtte.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbzabsyyq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guuozfxls.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gohkkynjl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdfoovfws.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvlxmlqlh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gihffnesc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gjzppxtqw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gacmkmufu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gpoktglbv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gntqtjvke.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/ganahrtfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gcqvhqnlo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gbrbwntvh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/godowsntf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gqupdvxsj.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/galzxsuph.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gtwjklmfb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gaeomixwh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gsnqkiscw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gzbrqaoli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/geexvmjqj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gbfsonhly.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gtvmcjhlk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gaqerqpuj.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gursgaepb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkndcdjwb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guasgzvmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gtauyetdz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gaakeamrv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnmmipfnj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gsrjcbszx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/giyxlzpcf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gpqbbclfg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gscfgokoa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbpqqwhxo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gghfgphrj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtwhhuyhu.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqifiyebv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/grdgfrmst.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gungstthi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gsktghlne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpsfbcgsk.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gaauqtakb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdsqgkhbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gakscskht.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtppiammc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gfojxxmmj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbajhslqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gungyigui.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gymevlbug.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gduukdqxt.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gduyryiyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gtozvcmqx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gtbftanpm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gdhffnnfi.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/goxoebvtp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gcscnujsx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/grvzvidbz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gwzhvwohu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gphczsnyl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdokpecme.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gssbedlfv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdztpaafp.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gwufsvann.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gtwgoeira.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkpmsgpkp.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gdxzfbvbo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gxnshfroi.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/ghxgcrzna.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gsgvnwoli.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gnrhiaxqh.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gszrwxtlr.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gevczcgri.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gcfiitheg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gucqaxmgx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/glvlojuoj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gondrqxde.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdoaxigoc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gdcmxqnzi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/glorvtmfy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/grwwdyumy.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gmxqilauv.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmbpoeryz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzqmyrduc.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/ggbvlhttt.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gcdqzckfr.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gbcbfnsnb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gkrsdnvpm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gpikdjqgi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gherfagro.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gthliwuiw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gmhaetnsv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gipasduep.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfopdbwvd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gufclxlpm.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gvpckgzex.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gzdzkuacy.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gpckaugra.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gwunhiuna.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gtvldwetl.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/guwrtexac.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkfkauivn.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpyyajhwy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/glcnmrxvu.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/geuldgbkz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gnnbaqdpv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gnxtsvdwm.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gbeeatoxx.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gmywcsyqe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gmhhfibxh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gyrntxvas.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gseekaqgi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghohaxvhw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghfytbcog.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gzmqlgkow.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/ghbgovuav.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gcjpwaqpd.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gvlzxrpkg.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gpfesfpkr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzqbjsk.sHtML


<!-- 参考信息 -->