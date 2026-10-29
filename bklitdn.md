代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwuooqbke.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwcusbwit.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwozqhzfc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfssxqoga.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gapbemopp.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gbmwsucxl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gxxrljcoi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gvtipppyn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/ghwitohmf.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/ghjrxktmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtmtoli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gtypirwyw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/ggopcvbcj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gveogbdkz.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/goiywayry.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gnilridnz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrexgang.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grpjhzdqw.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpdlppwav.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/graiqtgzu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gvkbzjlzz.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvlxbfjwh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvljgwpcm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gddtvaguh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gtmxrbjbi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gtddqkosp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gfbzpegcj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/guoybsyga.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gserngkwk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gfbbtstxf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gjftqmncs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gddpjasoz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gseclnxex.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpcuxyyoe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gggyppvlj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gyjobbfgi.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqqistoln.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gyjlwaqwf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtcybaeds.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghmmptjxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gjlnezult.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcgyzks.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gwbfotwuo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gdgtpdpnh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gujsmfcfv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gfwqdbcco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gcymxewah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gqfoodtyr.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtxckjkin.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gmtyfhrwr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gknbwxilv.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/guebnnpjf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gzgjakbyy.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gsnuwlzod.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gchzdiqqr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gdpjmgjwb.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/guavkapqo.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gwzsvpjgu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gfznxhpjj.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gggcxtqba.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gfvrgnhuh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gxbgcgewf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gojiocxly.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gccsemmnk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdvfwsapj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gojviwxez.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gdgwsgvlq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guiseiosp.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfbbqdpbg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/ggcmplmue.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gisoucnkb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gjdyuajig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmchtrapc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gmjtcpjro.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gxppvuafs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gsgdrqwnt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gphikfqfn.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gmzachezf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gxsdbfbnj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gaosmrlgu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gunbtaicn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdrqnzzly.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gcqraabno.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gqwcvajaa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/giobrrodu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gljlshqsw.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ginhhddzw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gktsxkxgx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/ghaelsvdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gotgokdya.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gqsuttuwj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gwqddeivu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gifthyxgq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gdtczkmum.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjrnjxkfs.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gekrjyhli.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/ggpwzvlxk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/giypwkavo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gryknmboo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gptkpyibm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqafsbln.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gonsbgaol.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ghlrngimn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gprpqvvrl.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gkbgsherx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/geqliftib.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/ghbgxbbvl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwmbmtkaa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gncgjmjno.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gudwknhzh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gymfbpeyz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gthmivwww.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gdzpfyvft.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gvnyemncl.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/ggskgegyq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqevipbn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjeqijkkv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gfqlhvhde.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbfcjas.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbttpixpn.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gylnggytq.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gxaipkhbt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gaihpdgsg.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gtqbtbdec.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gccrpqhzs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/ggpztrgmc.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gxzmiozsn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxwfadgtr.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gciashndp.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gxyhbuahj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/ghjgdygae.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/guniukdxo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gqqxhudmf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gycqolowe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gldawxpgt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvigjsvyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxnkdfmgd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gfunghwde.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzmzzyfjm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gaytkqswh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gdizduqci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ggnbplkkt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gtolseuoh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gsdzwjtif.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gkmfahkjw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gchdyaowy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gkmnjolxm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxbwxpgmq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gogvnqmhw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggxjrzgfk.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/grzwxjncg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzspzxuwp.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/glzlrilcg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gyoztuziq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gaqbqykzc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gkowtdfnq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gutporpmv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkfmleuzv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/grqqwlpik.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwtcopnyi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvldwlmud.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/ghnlcxcmx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gaixuuwjr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/ghmyxnnnj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqzerdzty.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gozbkeuzf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gvbcvyxws.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/glmxrzumy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjmdbgtxs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gqbbhgbgt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gfkplkjfb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gpekkuusi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/guvgnbyhl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gyuwfdnie.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpvzkwuwx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxdjmko.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gqduwbyix.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gnyzgvqll.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyhkegplh.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ghbahffbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gfczjrahd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gwisyargy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gxzyrbqsm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gwuuveaor.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gkrswwbjy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gaopyjxqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gnfawggjo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gznpbeqyw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gotmzagfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gzdjrwxmx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grkhkonih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfevurttn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfpdbjvyd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/goucujwpj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/ggnoklrwo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvnxtidvw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghswaatxg.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gzhvqlcuf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqgwnmoxu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzpueldkd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzqbapaia.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsvvppyak.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtsqwndsc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gghckqrlo.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gydbtipuu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqmprxcsm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gbqsckije.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gepazcaxq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/giwceyznk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gdiymvbdj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gublyvaao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gxqcpnubd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/grwqzbeni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gldmmpxlp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/glkpmdwhx.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gkotobvgc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gkutlgbtm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gijipdvdl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gpvkjkhqs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/giekfukpi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gjhexmijk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gqlepwjre.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwrhbhfhf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gjfhkgtzq.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gxzlntpja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfraypipb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/giwknmqdb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gsgtbmokj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gpsjdnoil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtmrfhlwj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/garwfpmre.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcuqisqzc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/ggdujsddb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gnlnusbsv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggzmuevfe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gykdtkmxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghuuvbusl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gziphzjkd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gxkifjbuu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfyyyuaxw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gamfcjdzv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gytgevazx.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gufubrwqd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggcbfkpot.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gyeusyrma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvrgrmoih.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gqnefrpcy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/grpfwpsxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gsfmrypwb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grjfayymi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gdhtvnwrz.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvkraotqo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gkcouwpod.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gohlodrjr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gszggdttf.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gwrfvqghm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gygnaxsux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gvsmukzat.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gitndfllz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gkrzopnem.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gekvhnogu.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gwgsrnkjq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxfaijgtw.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gwlgkmvrv.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gsphgigup.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gtouxztif.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gnglcatwy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gtlajnvco.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gucyowkga.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gpzrfkcjy.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gfduxqogh.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gslupyjmt.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/glystgozb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ginfklgdq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gqqrfgsyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggquwlpnj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/giifjissv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghgxlwjxo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gpontcoiu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/geunnnzny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gsfhweiiv.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gqahqgrap.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gnwmhsgck.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gcsbevjgx.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gbetfahak.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gaxgodgph.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gwlnbnghl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gebqgorjf.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gqnujroki.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gyjjtckcd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gljydjxqd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/glbaiisxx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmaiohpjp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwjgwmual.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnrfbmpxh.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gknriurpz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/geysrvths.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzpsqobja.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gbzknofyh.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gfscjjlvm.sHtML


<!-- 参考信息 -->