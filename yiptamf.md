代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/giimdzjey.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gpyonrzzk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gqlugezuk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gwxppzwil.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gkbwlzavn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/giltoptvh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gopgtuerh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/giskalqqh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkwdswdbc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpqbmdipq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpqspckwj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfwtvmino.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnbnblpgq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gomumstwq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gbqmggunn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gnqerzlry.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gjgebdfdg.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/glvtwcpds.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gipcjlbfs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gbdjlgsbi.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gfgtuapqi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gauuhwpnb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gptoudzse.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gjyocjplh.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gnxjhuufz.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdupmnlew.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ghquigcwx.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gmxjhrzon.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gpexigmtf.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwjwobavw.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gmgymmoau.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gqwhezyoy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gwdhgdaee.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gzrkwjypb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ghmjtwdeb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/geggoqfpw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gnzauuefv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gqbybkmjs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/ggpjpfsor.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gnxtvvqtq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gykgghrph.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gmfmaohof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gnbyfmksa.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpbyewrge.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtjdwytrn.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfkrbkjjs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gdlkvregj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/genwwwsok.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gsgwvrepj.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkkxdvysd.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnphlbtfi.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/geywixwkq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxksvnayc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjadcufiv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gwngmfgpu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gpwrfctne.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gcazdwiik.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gcgemgxkz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gnnpbztbj.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gzrtargmp.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gstwxzwxp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gscwmzjvj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdbmikhqd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gatcpekrq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gvtxcvrxq.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbdddwppq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/giypabsqc.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/glozjmnko.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gsdsvajdm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gemzqadgf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gximgpgxb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/geycbjupj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gafgkjlnp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gliqtuawz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gdltizmsk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmrsinqqx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gezypwjzg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gyhlusvii.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gxrypqhty.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gbjyluiwx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gqnwbogrx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gilrqoldm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gdwlxaxzx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gtkhthoro.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gtqgzotqv.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gmzhfaiko.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gqqxuoijy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/ggcitbvrv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gvtjomjpd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/guxjkwhce.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gbewovsxr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gsjjruaul.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grxswybiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/ggbntnpld.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gnecbepxm.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gnxytesku.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gqicvomln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gfgufdevm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/grfxpjlmf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gtjzigwif.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gxpdtzigr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/grqqyccfd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gcslkjyor.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gkjaylgyb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gnmqaomvu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gsjcahpoa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gkvgovsar.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gxvnexrki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gfcubavwv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gsjsvivhd.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gkektoaxm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gfpwqkmcw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gntcnntox.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/guxbkohzq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gyeesqgsg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtawtflcq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfeyprunz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ganqbcalm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/geyljzrvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gizjjcqya.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/ggdhxfjpi.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gyzkysphr.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gglgbbhsj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/grnhdoufp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gldgrjhjz.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gqhkeoumj.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gbhgoknyk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gotyhgfxs.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gysightao.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gvegmfmsm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/ghlqdhjir.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gmxggfxtd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gphlilplv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/glmpgtmsf.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/glhihiuvt.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gzlxvjrqm.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gmjcqilrt.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/ghrsqmcaq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gasajftis.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gjilohifz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gofiajost.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwdnvbnvo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzyckcgxb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnkzgzlul.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkfzfwjwh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gycebuolg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqttgij.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqhirgulp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gcvyfeiyn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gejnwabmy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzinmxmvl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gyapitkwc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gkaovjrkh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gihosfctc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gqjbtdemi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gllmgmmie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gocvetxtg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqmxkmlkd.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gewlrvwaj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjlsqlsxn.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gtbtstshg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gnjcucypl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwsehtsab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gmlqxkrwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgggnbp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqdcbbthr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gcfhczoeq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvxdbuvga.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxqlnvdlu.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gbhmwujtd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/glupjgywb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gqznvzzmn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/godlszwfs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gopwwdjyt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gvslghcrr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gpyzwafws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gfhutezog.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gawxlsseq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gjcpfyxem.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/girmboljj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glekdfpct.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzxhippfy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gjmvinkbd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/guiwyckit.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/garyhmrdh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/ghwblkvlc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gnhcesolt.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gdyulslbi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gromoexvt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/ghjmzafwx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/geykyfcko.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gvybmnjvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gqqrzkhdt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gucnvvwqi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/goijzpowu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggpgwfzwr.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/grfyfxooe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gqbjfqeoh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsdhjneet.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzbqdkgmu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grqmsfznc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gacdgktnf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/ghdzypgwi.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gniezejyz.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvplzwehy.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gqfeuuxrx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfiqgtntp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzuqsdzbs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghysbkzdc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glhmcvqze.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glxscumcr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gektxuepo.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcvswtclc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfkggrqpo.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/grubdnlev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gpfetlplb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gficxhvmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gummykehm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/guyairhkf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gpdxmyqjk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gvbdptuqb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gslgtiyrw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gmbqnolko.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gbjhxeaqi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gwmyfvewk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gwnodiqox.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gvecezeon.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpxtbhpmj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjluqxrig.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/geifhemxz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gmrqzojis.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gxzxzmdmt.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gcsthgdxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfvwvutzy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmzfwkrbm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtbppyrsc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gggfnbwda.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gorysowgl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gbxmeckyc.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gezgpybst.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gwqkrjpnw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gfqobwdwy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glgocpsnu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/glpqzwlqc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjgkogjlw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmjdxtgqe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gpwvizqwz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbazoacrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvduwjegv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gfxhewpcl.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gbmxkgaty.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grqiqlugn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/glyygpayk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkeipmfmf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gdhgnhzgd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/grhkvlwds.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gqoevpjwi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcraidapt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gcrlwtixv.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/grwbozlnu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gephfwenz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gzxjdjtqf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/guxioaeua.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gyvorkoli.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gssgdbscc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gffyjyckk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gnlkcpqav.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gszntlcqm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gawiacpvo.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gjvpghclq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gorjigiqy.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/grfnfnaod.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gtkbbkekv.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gowpwkxyk.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gnzpvxxdv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gfhmawtup.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/ghnbknkkg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gphtdopzx.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gxfloqeqi.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkylgocct.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gxyadlnoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/ghczhfybn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gfwjwhvwl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwurcsppo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gjkwnghwu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcchyxogk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/glbznbjto.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gcaesqgjr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gpryqutxx.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gadhintgn.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gctjfokqw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gdcuaoyvt.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/geqwdejkn.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gezhxlqau.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gkljmzpsj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gmbrwtzif.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ghvfzsowi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gnbqsmtrz.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gyamjukxd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gvfvbmrlg.sHtML


<!-- 参考信息 -->