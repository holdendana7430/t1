代发 wailian999

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghsitrzzp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gaopmradm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gcadcarfi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqqvosduu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/garsxufos.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gbzaadjtb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gnnulsaaj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gzrtzcwng.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gqdfaatnm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gqjphprfo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gihnkycuy.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gynsiuoun.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/glrhcbxfw.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gpfyvbudd.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmccuutej.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gqjrspupy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/guauubcwd.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gkgmuggve.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gxvqdofxf.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gmygpyvwc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gfxvmeyce.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gucwgzbsi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gieujgoif.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmtbwezgl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gcgqxyohn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/grevlkfee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gbkmcomqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gpjzfssko.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/ggjiewwbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfvcwhlze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/goqyyyydv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnmbytpgv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdkuoevsj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gknmlgrfa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwcxyzaml.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gkfnxtynz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gohvamabg.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gqafcjvxn.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gsfkfhrre.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxearhoci.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glfdabiem.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqlefvkot.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gkzrsqaht.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gouaajfzf.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gnqudanyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gfohdlcqf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gnxueemqj.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbhkcvlxg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gowvwazok.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gwetiseqi.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gtrlrpgsi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gudavmmjj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/girofbkyw.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gwbgufusr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gzcljbzuu.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/guafureat.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gdunbgcwn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gjmmlrfjp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkigffjaz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzkrlsv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/glhevhamv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gpfelfmvv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/grzgicifl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkykzcick.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gfunvkoqe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gkfyefzkj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gfxhjciqp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gvtuhwpzl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gpacejhqf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnogomtql.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gnoageslp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gbkogvhde.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjdrgkhcb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/givewyjyq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gquygjifb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gwjjyuqpg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/ggnkjcuje.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gelzsfykf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gaqetxerx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqsxkulfe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gloaqkwnw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/glkgsnuow.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gmvrvkyto.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gmvgrgeyb.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gbhvqnwfi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gllurxkpv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxttawvkd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/ggcopmwfs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gupivruox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gmggcfpum.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gjshfgfri.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gszdxrakr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gwlhwmfyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxiozliin.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghzjqogus.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gbhsatqts.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gsjxmfbmb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gglrzbxoc.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gukyuadbj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gxohlskzh.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/ggoyfohdi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gpgmlvnuj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gtvvogspl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqqfluskg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gkoafuhuz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfswccqbj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcbimeczd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gzjuzfbrz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gpykbntwc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gwrceztkr.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/giyndtidb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvzfjvrqv.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gpqgmgepl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gbchmzfkf.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gsddxlxfe.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gnsemkibc.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gjbdfxush.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gwvwqamyy.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/grmxgplqf.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gquujbala.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gdqdayjhs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gvrlvmjrp.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gvjvafhgp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtilbqshe.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gefybfoqi.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gmeqertsx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gosezqtcn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhyhwpo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gzrkwygfw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjsmlcmsf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghfzgodmz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxhlkdnnw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxighjnxu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gkzotzhuo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glrfjrete.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/grtwbxwll.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gytosuhvp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/glgrxxmxn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/grecesxme.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gjuntkixs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzsbmuaud.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gvjcvoqqs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gldhnogza.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/grwgqwrmu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/grodxikjc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcjjtnqgo.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gtuqbdkzw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxudkdgfv.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gioudgged.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gvyijuqvi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/guwazwiev.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/grfrbuktt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gcpfcwwgo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtpixxyad.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gipkybnec.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/glhyatxry.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvnvtgpfd.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gkkdvonpf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/guuxpixkx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzzlpitq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gwhlidmhv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gdsddxudq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gwxtqfpye.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gpejhnvrc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gyyadjikb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gmmvwzqap.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gulwvpffo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gvmglpywj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvfwcnkrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gkkmhjyym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gokzrvcin.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcydiqlor.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gaahialku.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gbpoqpkbu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gthdmxmsb.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gnqldxtmx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gcyjuowvy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gsqibmnmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpztohrjh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gijaejbgm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/giduhttvy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwbwprflj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gehkjzhhf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gnbndgwvg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gjkjcqcgk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gnmcdqdmc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnonieefz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gabxvmnsa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gozssmpuc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqshkpwqu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gvyisevex.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmibwkznr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcsyzutdb.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gcetyotxh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gejisksxb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grtrmpifl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gigjllngo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gokfxeguo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqeocquqe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goxkjxkbc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpkxqrorb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqvvnbczd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/ghwgvuksi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gowztptko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gftgdtlbt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gevenhftq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gxbmetezc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gmgepwkbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gscqdkbdm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gccavajji.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gzsdyxogw.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/ggdlnxjas.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpeplmhhb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gfwmfifme.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ghzehyqwo.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gcktztqep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gfiztshgt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gykbblxfm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/grlnjddoy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gjqpccklb.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gjdmhbuzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzqwwuywo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gggovlgdw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gcpbyjdam.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gglyegynz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grusgcplx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/guwxfndam.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gztbkjhqt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gyefvaoyt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gcgcviefn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtzjnvbrm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkvrnojty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbbmwruqy.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjoiveldq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gtpsslpud.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxtwfmexa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdahbzhsh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gynkgcupw.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/goxvvvfan.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gsvkkwpue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/ggykkljqa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gntiuitvj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfbzjwduw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtjbapizn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/glibjrthe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/geqkosonl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gevlccszd.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gqyaudgym.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ggbipvnpf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gztctmpoo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gkqxfuhjf.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gczqunhmw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/ghwzlryvo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gnrcqpiis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gkatozeoi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gvthdnrec.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gieejkipi.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gxbfwbbkk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzyxnzdfs.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gmnqlopww.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gsawxqrrl.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gamylvrjb.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gkkepvghr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gjzixovpl.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/ggiiddduv.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gpnmybbma.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/glojmzrmr.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gohsvepef.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gggxmuwfn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gjjmvnmhq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gzjndnygl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkdtijxdw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gopovvttj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gredqnpzp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gdaxxjcru.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/glmctvnah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gecnjspdk.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gbxepllgb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gujyauuzv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbptagilm.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gnfqggftf.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gvqnxihzn.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/ggrtycdoo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gzonjyqrf.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/grxjpsekj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gjhniftkm.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gdkmylgby.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvzhmid.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmfiwuzrw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmynrzepm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gnxugkgmc.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gzkwwaagj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvmubmssk.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/ghvagvmso.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gintpdyca.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gpsjmtsmn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gqxfbmksu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtryaqglv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gdlrwqdrk.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxouaktgk.sHtML


<!-- 参考信息 -->