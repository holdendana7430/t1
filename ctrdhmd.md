代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/glqffrmnf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/guonrbgnh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gwgxiwoxk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gijcgkspo.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gfoswqksk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gvtgqalhv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gtucpdozr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfcuwivbe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grhwjhhay.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gexghhjar.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/grjqxtcen.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gznfzmgri.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqeagvbxf.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gkvbpkszr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/glwnoyinp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gtnmeindz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/glieotoct.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gwelwmkzt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gyijafzkf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gfysfwxqh.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gswdsybrf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gycjvbnvi.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gnffaflld.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ghndtrvxz.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gasclyfbe.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvqmwkavs.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkddifxny.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gztzeowtt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gprcclvmq.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghbhqdhay.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ghjiyswru.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gogtcewyb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/grtgydxoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gvszmeuhr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfvlvmygb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/glcqrzigf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gwjpdykfa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gdgkvuogq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/geafltiof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gywdpohrj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gweothdyn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gupekhoyl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gjsramckk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/govlhcrmp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcwplbfob.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gluaarsoy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gfvftkekr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gtsgzqcfn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gikmnfywe.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gecfypclp.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gxdinfxhs.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gqxbymypr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvtwxtmcw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwtqifukr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gmgrfbbcj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gusgdfxak.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gobnpdvsy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gyhtiaboj.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gtbqplczx.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ghdlqvxyh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gfadfhvby.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/ghamnmudo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gwhecxhwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gbypoekgq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gswbwjzmv.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqtwvfeze.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gaeibczwy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gntmmhoio.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gbjuihtdw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gdcomnuac.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmylbzsbc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzhjdainq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/giufztudz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gcpvkcdch.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gdxfwzisj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gcnnverzj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gfsqabggq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gaywzprtw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/ghzqjyeuf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/ggmkwosnd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gtuyhxpoc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/glxcjatvp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gtsegykqt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gyuqvvlec.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdlwrmuor.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gnalbtxcn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gctjompmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gdnyyedlb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gqenxsaxn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtuzcmlnn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gewowicee.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gxiqnipsk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gyzmexjwc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gnmmqzwem.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gzzynlnip.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/ggwblyxgu.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjhohzbfp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gqrsyeupr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gyweqcftl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gxbfyfkbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gprcwjphn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/givyavjhk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/grtgdnpac.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gljuiuvox.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gsmlwvqxy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/grbeeenid.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/glslrhwmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/ggekpkxub.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gqtoqoias.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwfkfhkvc.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gtafuldzh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gnksgzndd.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gwriwgegg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/grxhucivd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gjdqehrta.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gpifwxgfb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfswujnnf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gpzqniqrc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpzigufxe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gmcsgfubo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/grofyrgnc.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtkifxhmt.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzagqjj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/giodjcjei.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gcflzxitu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gfjsqskxv.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gefuejgfb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/ggfbyxmwn.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gallwwkks.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ghlzvbqnj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gtdqgolqj.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gxmzvlqya.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gahuiiwji.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gnwtyqgsz.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/ghnhiwrix.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gaeqwknmm.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gzgrodrzz.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ggnhqwmom.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gxgxzhzlv.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gnpwyptex.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gmkvxdizm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghnyxumvf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gghuyfbdd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glxrpphtl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gslwihffu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gnxiqrdcs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gyxvrospc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtzsbhgyv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gyvvhgzpq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gzzrlufhb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gghglkybj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjxjdgtli.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gipqjrrnt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gyurzsial.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gmrkatgxd.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gatljnnac.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gzxfrazdb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbumzpqlh.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gvdyttbcv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcnxrwulu.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gwuggqecw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/ghgilkazj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtcubattf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqeieym.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjjevvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guulzxlfe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gkgihsxoa.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxjybgcsg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gycqknhgq.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gccpoeqan.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ghtvdmqnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gzhitxteg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvgwhnqrt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gnfxfkolv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gqadecxos.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/ggqfpigbo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/guhgjwmwv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gqxparnil.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gjmsdepre.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gtvustjni.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghqrgggup.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glqmshrca.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gdkpgptue.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/grmzeusnq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gsbrzwujg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gbainamen.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gipiishyg.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gwitvolia.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gyfjvnwve.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gusqynuqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxegugssg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gynszmlnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gpotichra.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/ghgwoxets.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gujmtylrp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gzuhssubo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ggfkamakl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gydrocheg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gahucjiby.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbkmfdbbg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqvgzchgu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdciuyeus.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/ghyeicnyd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvgixwift.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwynrfmxt.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ggavbxuet.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggkrwmvbi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grrzltuww.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gndgrauio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gklggmevr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gytopvpuz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqwtrrgyr.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glubkdgdq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyefgelub.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gjfbxayjn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gevkefvmx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gcouylzgm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gpvthxghn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/giuegbcrz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/guqlqwdcj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gmnvziwbz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/glvahifar.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gglvdojwp.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gidbyqtit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gigmeavws.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ghmnxkxja.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnjcdkd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gntaoqbwf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gqnxjnmni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gilezbttj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyyhdpvra.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gezqqjhnb.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/guyawnzys.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbhogawci.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqfwubxrd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gnbdvetcb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/ggjhkymaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gneneqdoy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gjffzgyte.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gosrjephx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gguosrpic.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/genijnywd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gixiipago.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtgegdosh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guwzcrpwf.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjajaulsv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gjliktbkf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grizghwsg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtuxksknd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxuffxcyx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gfoleyovj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guluolfho.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gploterur.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghpgbhnsh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gefhnhwec.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsrorqawg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gsilzlzck.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfdzwlnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gaxghxghr.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gqwporrdl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gahmwdncl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvihqqbbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gmtppkumv.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gmbecsakn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/godskvrqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gtuubrkkp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gvwsxcdqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxgxnxapu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtasxsksm.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gowucdqzl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdujaurbg.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gzgcmwcgk.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gwbejhyzr.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/guhcbwlbz.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grnvfhwhr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gaqhawtve.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gensbvfqs.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/girtwqdlj.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gryuadscy.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grdkbrdaq.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gngrxgxqe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gnyuvdzhg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gyyqwugno.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/groujmhui.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gfyxwpcvo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzpantka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gsejigcpl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gzsznmchz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/galoxubzo.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gucjbxgtq.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gxdslhkvj.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxtulqpid.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gcosdlojw.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcwstrkkk.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gkdeeamzc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gbyygbaho.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gzdyahdfe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gtxrluuuj.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gdyfrvvmy.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/guzesolyt.sHtML


<!-- 参考信息 -->