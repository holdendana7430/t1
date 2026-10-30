代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gisqxcitm.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gsuvqfwly.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/grhszhmod.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gnfivghqe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gryjvbpua.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gtbvulblb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gptokencj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gymibiwjd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gpmjapxbi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/geokvopec.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghzcrksny.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gheelalit.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gywkunwib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gexfmqril.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gvkkygktk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gbbzoanom.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gokmyvgrq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbetcaxnx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gmujzspoh.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gnlaowmjx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gdcygjhik.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gruabexex.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/givstdkgn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gardvktog.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gwkowavgo.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gihltuwxn.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/glssjbnmj.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ghjsmfclj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gietdxyhy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gemguyias.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gznvufbyp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghgimjlxp.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gkwcnvhay.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/glwbfrjvf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnkdbvygn.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gwtdlylhj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gjeykhofx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gzfdxorpl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gdarcidqb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gukcqnaxa.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gxfwfdfqo.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gsrlcsrxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gngayaasc.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gvpscazrk.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/guswrskhz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/giyucsbqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggwsniahc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gdsgjvccd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmogeysch.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gnvbqiavn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gsqfrycaj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghmfvluec.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/ghunaykze.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gujblfywf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gighqdlul.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gdrkqpwoj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gsiuxqqzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/guavrymgo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gobtcwvyu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ghpnjjilq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gwajcrfwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gbiraajnv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gbvlbkuhy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gbjaekfuu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/ghsjthdvc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gftuxbxng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gbzvjtbpx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gdyqmyprc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gnxqyigwv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpafsnong.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gfqsdsysc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gozbrvftn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gwxekjsmf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ggiuuqbns.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gndocybkh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghllatdhh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/ggyhbfuer.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gdhmsulqw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gzbeysqks.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gpnndehql.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gytqtsvbk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gvyhwfpfv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/ggeykuzxa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gbrrmkwir.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gkydyblnv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gwjrplexo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gaqtcalrh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/givmzabsh.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gkcgmczxz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gnrlvjbiw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gmbdgdaoz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gkqqspctq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtcertflt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxzlfitcj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqspxrjcu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gggjpbxxn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gvbsqjysq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/grgfcurap.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gjkodtweh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnwixbtyh.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gwitnrdrt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtnfxchzg.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gcqmwslqg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gguybmzik.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gbwrgkqeb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gvnprhwoz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gutlhbuxo.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gjlhbrsml.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/givyliqlr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gljdauwol.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/ggrckqkcb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ghupdpbkw.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gvkfysqbc.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gzaclnvpd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwshdpjnc.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gqgdomslt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/geuaglgva.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gfhebjzlw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkflbswzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghmjnrjuo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grryeuzlo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gnygguryj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/goozrewwr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gucyequao.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gcchbjtsl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/geocojttf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnilgnlyk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gjdgxqyig.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggxvgexgu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gbigqjmpt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gxfgxqpoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gnncnjdra.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gpfchjqww.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfkbicxsu.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gzsbrrmli.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqbbwlsko.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gonjcdykh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gkjdauqkk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/glpbaxpvm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gzylfhgvv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvhucesdk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbrjmafhw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/goqorzdvp.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbglhftdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpoxmcbke.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gydzvyayb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gqhbrfalv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/guvoyjxjd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxaljakgv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxnfnlbnx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gzeztoeco.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ggfvgszfs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gtqagegwv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gkuolxbyq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gzkrobngm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ghsfjinuq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gbdbmvhbx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gfgmbhodc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guuunzzrm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gwrqpxnqp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gkxfientd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gwxmgkzam.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gagdrzdgs.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/ggdqfkqkm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxpiedgyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gplrzrhyj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gtfdcciht.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvdpzwpzc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/girdqbgqu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gpyxemfln.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyberrvlb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gjigzafxs.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/ghmqwspzc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gckpgrjic.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzjulkqje.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guqjgjynd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwmbtxzmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gbgpudqpn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gqrgmfooz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcdmeueit.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gglxlpwhd.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/ghjqczmet.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdykecxtb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkzjqemks.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grveufryu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvgjdvo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggrnawkwu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grnwtqmsu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtprmpluy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gniflpbbc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/ghafedbfu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gcyebkdqz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gdmejnuxq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gjieuzvvo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gzxfqddrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/guvzzbmlt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gklgdbnis.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gcknzybnn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gytmslayy.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gwfdutlrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gyeocldsn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gjmvlxoku.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/glbvwesry.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gtlebrdiu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gmqrmcwsd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gfyesoxwu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gljnddzsw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gwjoanepn.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/glgkcanux.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ginjmsfqx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnwzikrqn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gruiolspn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gtccmlahw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsdhoqkvs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gybizfjlc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtyjiqznf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/guyzqtlih.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gxrmruehq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmzlqfyet.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/geddgzrkx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmqncisou.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gobbdryfu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/glaaiisnn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gctlpmpyq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gchvxodan.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfhdfzdjx.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gdtbnkwcv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnkpecfww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gcwphgknx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ginvupyyk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gauuvzrek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/girgkoecl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/glchbinij.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gudzifcgk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/glqyehzbc.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gkexpapum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gfewmzhfc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gbfygzsoi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gokcfilxn.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gycmfykzi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gaagbjfvo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gabswxheq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/ghuzxvbov.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gccsjiiph.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxcilnry.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gacycwaaq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtzmdzfnh.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gmipfcpuw.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gjnfhvern.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gofctxlva.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gzrwjlyjx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gxhltflpp.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gsaqcchwe.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gbcbqxgzy.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gqqaspjvs.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gfvogutyo.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gyomhzxit.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gwmlajcoz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gvlxqcnid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/giryazbcu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gnwokzdxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ggfgspfqz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gwghiujdl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gcqftysvq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gmqndtnnx.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/geohtsxjb.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/germxtypa.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ggfpwrbgi.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gmsgoicqh.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gkjrhzhis.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwozcbssh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gxawkpspv.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/ggydrkbsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gkojqsksb.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/geqledfxe.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gtfpdmotu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gcjgdevik.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gfrkmmmqk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbkyrzdar.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gppswnftm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ggfdlbfuo.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/giocqmrdd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gvcusjdaa.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/glhjpkojg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/ghixblabj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzblyepdb.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gfnpiifdn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/grgdcbzkf.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwkrwqwsn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gwrggiflq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gikkzsgqz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjuskspyk.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/goffnnmvb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gddaxudlm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcgynxmzd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gcqtxfcap.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlblobv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfkwrjyrz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gvtyvgsjb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gdfjfhoey.sHtML


<!-- 参考信息 -->