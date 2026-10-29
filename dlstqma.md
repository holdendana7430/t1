代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxmprxlkf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvntebhxr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gudzoccgp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxkduuydn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtzxyfphp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gkuzbdhbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gyebwmbfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gxtmglbau.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gfniiinra.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gpmmxvttj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gbwltiomw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gdsyacqnn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gnsjrodjy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gyjifqrjq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gvndnmojh.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gjpqpdwlt.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcivjnp.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gnqsehesw.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghrjqnkhn.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gqzobdged.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/grshdqulf.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggqwrfgst.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfyomlnlj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gtzgrfpvi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gwoxlcndu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/ghsdmqwnb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gynscrmcg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gpqnmwicy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gyemwrvur.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ggwpdgtad.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gsijpabld.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gytntyeof.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gvyfacxgg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/guamrgxwh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gaufqwnyg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gldeicwon.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gctvxkezj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwvlnmlxo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gavxnwdym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjhukjykt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/ghexbvcny.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghnuckcej.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gupmjrfgn.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnfprxwyw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gcffzktar.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjieaqaqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gjwrmjpei.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/goydmphrr.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gwjlfgdym.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gfexdtfsj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gixmygnjc.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gllvqxcoe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gtvcnootz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/grqkcbcgd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gxlvqmskk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/glsiadyhf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gkoubgdvn.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gidrtmgkw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/grkxwueys.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/guxiospxw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/guaiktfwr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdubjflj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxkubqvcu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/godokedbe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gvlojmnqe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gtchndxqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gipzlegml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gvhtnxrap.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gatrphalx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gasxztxam.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gmtyiplns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gjbmwwnwj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gibulnmep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gybnpibei.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gkayhzqzv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gncgrdpjq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gldhmyumn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gayszsodd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfanqrmrm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gpgdxygtq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxrgljs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gcvsvxinf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gilmgatyc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gtngmvmbd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gosgcgefq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gyxrivpxg.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gkuwoollq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gqesgtoqt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ggjwtompx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gfbmwnpeb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gmtjrhyqx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gwgbqksoy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gmzfjjuis.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gackoukjj.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gpgnrnpci.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gcorhnclh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gjhlyqbla.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gdvrlrhia.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvdfbejih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gsbihbloq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/geequppbi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gcrjsdyvw.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gwlnpzsss.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gvjadiygq.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gswmwsdmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gbmnwikjq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gbaybxafw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwlkyndya.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbqifdcsv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxxjcgeuq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gnjixxryc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gtctaiwss.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gxlzexfcv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gzugwqxgx.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/geubihgtk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gnsvhrljk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gknebzpvj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwslznyj.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gwwndotzh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/givfyklok.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gmfeqwpvl.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gguvehpqe.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gtraebvea.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/geswpxtsu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gqwgsuqox.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gnhrbzizw.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/grahnnafo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gxcpzhfru.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gpwskgldb.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gdqpfbpwa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/ghmoalbbd.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/ghednkoiu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gdomrnxnr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gymuksxon.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzrwzlhhn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grzmndnjz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxbcjspeu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gjxzytdjg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gsggjatxv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdmtlmoql.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gonmcfzdh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/giouxntpo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grylsbrfl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gwkjqelhw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gyrannyfv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/grofpzfcu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gfjbsfbdd.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gtzzaamif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gsjepycio.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzzdwggf.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/ggtmhqktz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggqhenpax.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gkdjirdnl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjzpoblqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grwzsnkmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gcbibjmsd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gmdaxncoc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvjhwclqo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gjyepuwsz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guxxlsygp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgzhpwu.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gxnnwdugg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gfjcuiggn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gdbgkrjiy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gtrrofeit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gntueibcx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/goluthvuk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gdvzmkxsj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gnpoqnzms.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/goepjcoja.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/ghfvmxsyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gxynisets.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gnllollvg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gfatecdew.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzrmgoaex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggspbrvnm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gzvpultoq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/glcejrqyf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ghllealsh.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gcwomxwxj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/grczhcydc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/ghajaedej.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/goockxtxt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/glqimnhoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gzfhtnmgq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gwpjljgcd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gzzgrkhtq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gxtiiwbck.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gbuiqnccc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gzylgknri.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkwkjmuaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gffouyybn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwkmifyed.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grsloplcm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gimtiqayj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnbwfknkd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghtoenroj.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gyoishsjo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpwfsvaet.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gftekesrh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbcufvryn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkmufiadl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ggssaysmd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/guufjrcrn.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwtudowpk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjipbmquc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnqmcsoiv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gpxdzziix.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gyuklrzwt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghqqvyvkj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gqzydwcgv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gqaznkyhc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gtvfnknrk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gtyersuby.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gtyorhoeg.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gzokrouuz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gtubothcg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gvhdyvaou.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/genhpjxqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gsknafnga.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gukfuupsy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkqtwuvmv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/goakncxnj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyiceldmd.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gmmlknsmp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnhyjcnxg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gerexenkf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gmtdawgja.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/givfcosvz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/glqvyixvv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gckjlvbht.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/guahvzais.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/guhheiwyc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gcxdwtcip.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goikhevxm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmjgimjkv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbtavzhdg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guvokgamn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gzaekcwvk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkzpmxymp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfvmlnrze.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtjrvbpdv.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gfdujkawb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtfcsntwp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghvebfsxq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdebuqef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvypqwrma.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gehamuemp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gndjzsrhd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gntoqjbwq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gdqzzwlwp.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gxqtmmmuk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/grlrofnws.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gyfqbgahi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gfvlpmrgs.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpgbgnx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/ghmxtkxes.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gxohvvloo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gefcumqns.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gphistdak.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqyfzjdpp.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gxkrcuhdr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjfnihmyw.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbshvurdc.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gmnqmcirn.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkozyafvd.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/guobmlqyu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/guibuyxhv.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/ghibliugp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/guslraabd.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gjynasxrb.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gyxjzihvb.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gmepyjqcq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gflplsmdp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gqshdsjgu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gspvsicqp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gzapkdles.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwrdrbesb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gghlpdxov.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gxuniqejm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfmfsxlsp.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gskwrlvfs.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gmpdblnas.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gbalikxjj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gqsvqidxu.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gzclddhbr.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gyaawzzcd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gihmkxwyr.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/geragpgml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghypqdwbs.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gffyinduf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gimjnlqpn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/giwarfwbp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gupctklcf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gtlnsxzbk.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzskmbqto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnnmrmjgq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gzvadqcwu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/grqqiwjhe.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gfpnvgqqq.sHtML


<!-- 参考信息 -->