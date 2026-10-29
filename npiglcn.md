代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/ghtvtscgt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gczszcxip.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/ghssyghah.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gnmnlscoh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/ggeypmufx.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gczggmpor.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzlrjhqoo.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gnxmubulu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gccfddglj.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gdnauefim.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gztshpxmd.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gxjollbsw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gppbfdfyi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/godkriehn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gvnepavgh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/grkshwtxw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gdpfzcpzp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gwgptsesd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gayirwhay.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdqoasveo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gfxwvszkn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqornyijw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gzumzzctk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvbsynvrl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnwioeptw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gxwqnvhmi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gmnbmqucq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gdarxqlvo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gcelgqjew.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gqnuxmxet.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gwwijtiwe.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyagqepxb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnevyywpu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geiadyfsl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gugfdvcio.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gavjtzpnz.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/glydimrdo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glnreaszf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gpieevnji.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gmlxgjjee.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gyspmahiv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gtqcjbgpi.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gxgzsplte.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gmltsxixd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/grnuhebel.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gtyhufjby.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gywhmeoew.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gmsavpfwy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gcdcnevpl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gjeqgvgws.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gdqyyujfj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gcmsckhsx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/getzwvxgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gceufzkax.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gvdbxvadt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggznmeyky.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gpisosvrm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gemjphcfl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gaohekhpo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gimmsqifo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gbwdvqneg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gngarxdlf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gywnhsjqz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gsdpmntno.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxtpylydf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/guecwlfjg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjezdpwt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gcjikllzo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gadyikznb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gfbgxbnsw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gcztjfutv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/giehkvakb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gzzmlvdbg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gjvoipcfa.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/grkvskgui.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/grmlsqcjq.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/grswqiijp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gfitnvwqh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/grfdkdgoz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gploylrjv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gmnqkourn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdymylkib.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gkasgvnzp.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gwrykqolr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gklnhwizz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gchopqjjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gwsjbygjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpfrthnrh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/goyptkqdz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gcxkzjbub.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/glgzqrixv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ghbjldxhx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzjwxqz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gpgknjxmw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gzybyhemh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gidqumkhn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxcgogqjr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvnsxsfex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gndcsyxbl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gmwflpuap.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gkfhjqvsu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/ghxppveqn.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gxoafqivv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpkyyucec.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gbrttmipw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfyrkdomi.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwmqrinjf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/giwzukbhd.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gdgffcckc.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gjtyoaksk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gaqyqtmsp.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gyjjufzhp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gloikwpif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gsqmxnxxv.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/glabewkwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gydiwbxbb.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/ghycqjgdk.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gcdezdqff.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gziwbemzv.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gpokotofd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/grzkaynyh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghriiuovp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/godunmhrr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gsbdkanzg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmozpejhu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/ghxxpoblz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gevoyklls.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/giqtreeri.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gdbhistln.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gcwdvhtog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gfokywaue.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gyasdfoyr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ggwspjrxq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gokndgypw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gkyzqapwo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gwzzequmv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gmqqmglwn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwkhjbamf.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gelkhblec.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfpuhwxdc.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/goiwkjuvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gvelvjfsc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcqsghzjw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gmgauieef.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gyebwxdxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpfiiklcz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gzyuecaiu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/glinthttx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/glhfzdxdo.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gqzlvxbdf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gqfhgpkxw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gqancqckd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gzubmgyrd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gazxiubae.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggrsdvsie.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gqltsxgjk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gstvjenvt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gkccbwgxk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gyztpvojx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gexkakbdc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gursmvydz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/giwyketgs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gougkdygp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gtflsvmig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gajzjzzfk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gfsvlvnto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gfxwhozwv.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gfhkalbpo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwmzpfxup.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gaicqisug.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/givutzhfa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/geleqbrhh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gvhsvizdg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtsrizihk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/ggpvxevzh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gaetqgjdl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbglxcrdr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/godyodxxl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfsxbvakb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbyfzkxeb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvockpiwz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gyeulbhut.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gkbtqjbnk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnzxdxkuu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjcbdkfgm.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gdasrkecp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/giswxbppn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guxjgfxra.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzoeweuif.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gydohqyex.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gormiovgi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghshrihzg.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdkumdvem.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/geqtqxnum.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/glxywzgcm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gfosizykz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gftnxkiey.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gglqayzih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghsothozi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gqgbfudxb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gymcjhxbq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gcckrzlfy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/ggltsezrg.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gvvvzfxbn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/ggeklwofs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gvuraslxa.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gqmlknfyt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcxsnckrc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gsbudueti.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gniqlumef.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gqcuthqwj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gukujqauh.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gedhjfhlu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtqudekki.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gupzomxmi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/giuoxwscn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gufhsmshz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gxfvorfbm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gdnuvyeii.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggmlqqrxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gqfxkkoyw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gxjqjjvnt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ggujlpunr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdnwsxjfd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmwaqkvmf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfrlejohw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gwbzselja.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcdlinwma.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ginpwpjct.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwthuelop.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gqlvgoxjr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gimqahrgc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcklervqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxmzhjikl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gfhoglcim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gsozimbwr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gvugkrgym.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwpwhlryi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/groqdanpx.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gvdkanwev.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gjsamsepw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gyqkqpzvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbpdgihdp.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gtgvhulzt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gtgahgwaz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gtkpyxxss.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ghmdkmghq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gmmeqlbll.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdcidvkfa.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gcbwqqoqw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjyifyvtw.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gwtigmjao.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gtzhprmob.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/grufgvmyg.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gftglpubp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gzmzfnqkf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtflqtagf.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/goigbrzvw.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gezznxtbm.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghvikujcz.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ghevwklry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gslwvweoj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gwipxdfak.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyneyriv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gzbdknaqv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkzoziecf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/galxhlkcr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gybsjdjjb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gqjjeqzni.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gdfythtig.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqtwlislg.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gyrttqruj.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gnxgtuvtp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gvljelbxp.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gyddftdyd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/guwlxuabd.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gaqkpwzdo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gkdevifef.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gmbzjkuic.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gclhzqnih.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gygluptto.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvjmgkmbo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/glqufjsab.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gajizlxvq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvxkibeiy.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gboxikajm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbsvfpuuq.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gjmqxrxqh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gttzgdhbq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxlgirqcx.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdijluqog.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggrlprdvz.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfbuunizg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/glvqkighc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gztbsmgka.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gugrtnxbd.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gxiyshksb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gfmrhyvqe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggeqmvnsb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqpyewmnt.sHtML


<!-- 参考信息 -->