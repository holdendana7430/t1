代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkcfgqaut.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gougjaihc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gnbssfkob.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjnbcxwxv.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gecklupra.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gbbeugais.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gqkywsaoq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwersuxme.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwiqtsoba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzlnudrmq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/grysaqgqn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnfiroozr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghdryadmv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gxrlqizsh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gxwhnaaje.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gokhkcbnl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gneysfbqr.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/ggroeeaii.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gxdxolcpw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gszokmuqj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gheqyxqbv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gmncdexkn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gpkoefyaa.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzyaawbi.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gikymbduv.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/grpnuwzwx.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gouyexarr.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gdjcqpuwu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gdleshoan.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/golajnorz.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzqnddoqe.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gjlhsirrr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gomqnxuvy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gvpbncqmp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gxqkvxrag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqvkznoqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/geoqmaeke.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gnkpjpkmt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gyhpkpmeo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtbxcglcn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gudtqedlj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gkmoclake.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbwrhzhid.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ghcafoibl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmaokayvm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/guljfbltz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gyzyjjneb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcsbuogft.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gxdilxwzs.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/givmelbmt.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gqumjqmrv.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gponekrsu.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxdslnbxr.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glqfzbxmi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gagjvwgnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/giygzgzmo.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gkunyltvr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gyngabscn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gctxntyhr.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gmmazvhyi.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/goyvjieuf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwofruwwq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gcjhpjabx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gthllqnxb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/ghmginnim.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gdjbihndt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gyifxgqiy.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gibnczgec.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gqwcuovzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gpdfqnesu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqebkcljk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gnsyvpqjz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grktyllwi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gdlkehhar.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gubqttyna.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/grucizubk.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/grzjplidj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ggbvmdtmc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/glwgyugmi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdgvsrffb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gqqkcqawm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gyxjpoqnt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gnvkwqjpk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gnqwupanj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gzeziajar.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gjogqoxon.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guwheqpgz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gfmbitgus.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gcnzrnpql.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/geduujmmp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gazkshfpe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gccljxixk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gcgzcjonz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gwzxyatel.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gjtcllytz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gzygruorb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gggdqmlpc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gufcgiqmr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/glwhfagov.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gowtdggwd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/girzxknlq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gdobbtrjy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gxcexkwgb.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gdmiqbmna.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gzsceqmnj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwygdhfhw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gevtlmihq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/guwlgjlef.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gjraurzjl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/grodhcazo.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gkfvfszsj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gextlsvca.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/glndfibnn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gmgmwcfuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gwtcrnmhv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzikkcoo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwdditvqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gacbohjvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grmhnjuqo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gxdhqkqyk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ggwkdxcws.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gyaacdbok.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gcrvjbqxu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/guuqttclp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghovovzul.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gwuvmtwdl.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gggufwzit.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmawozpxu.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gqbgxoxhi.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/ganqpcrmr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/garcptmcb.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/ghpoqialt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gnsphrvax.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gemfbqzgh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfihdtv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/govtfxacn.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gbazddoes.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsibiug.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/grkcnrhhx.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gzlgmuoif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gktbxgzwo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glzqnppvu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggvyhnjwx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqftulcrw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfhtqjgbk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gtvhusyac.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gihrmbvld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcmgeldkp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gnmafsgvx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvuuvnz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdlkrmirp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gupihmmpn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/glrnpxlto.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gfotocydr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gkbeubeix.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gkqoetvob.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gxzujavwb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grqxuqycq.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gcmsevryh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkqdxpagr.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gjsrqhekb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gahdcqvgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggvvuonyj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gjowslwap.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gvbiytzjl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gqhachozk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggaiyzngp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggwuchomn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqlpjjsnx.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gnxtpcmea.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gnkpfodeb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gndiyubnc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ggiggxgws.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gzbabekmj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/galmhsuoj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gtkeavgre.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gxvdtxzpv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdmylpfmt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gfdiisnta.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gfqmibgdp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gktvoqwrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gnkoqevmh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjdsfvbuz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/ggzhgdbft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gpehpyiel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gooowyavt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvmschumj.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gybdlkcyn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gpthajhof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gdyhtydyf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gxdwahuiz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gfjahufzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/guqjhjrfm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gboxrukru.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gjlaezkmu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/glootfcwf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gadufhkip.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gtmmyrgpq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/glotbradm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyouhqbgm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtnxctreq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ggoxyonjo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/glnucxmfg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxexyielj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gowrrhwun.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gbwsmvqsw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gumysqqsh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gztquxujs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghkcifjqu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/geuazkkay.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gqsifymli.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/glmzmrkgb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqdhxyrtz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbekcptie.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gjdmjpndp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gfehfbziw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gligafmgp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gddnrogvl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gwxlalmgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gvujuoacs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/glzefvqoc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gzxeyxxqv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gcmibzcxj.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gkuhwavsg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gkxnaafit.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gahxgebvi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ggntylxcz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/grjnvbdhy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glfraxenk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrufjzim.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/geenwpzdj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gjayqxofg.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gdyhgjaum.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbpqrbnwm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqkehaxxi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxdvwbhcu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/geqymywid.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkjvttmfr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gkymtyhzo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvdwcrukb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gqzrrlfbn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gktwwecvr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkvbddhbd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gongntiyb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggnuffavp.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gseujxmzb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gpfifnfgd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtpaqzhez.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqjvvjfcj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwmfojgit.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gmnxbvcvl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpdyxttgz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gcmgxwmut.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwwggjzie.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwglfaycb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdfbkwnfa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gsecdzydf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnvcxhkmb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gncwfvldp.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/girtwpyuc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gpgthknul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gyhnamtvg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gvuykmgum.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/guugoepsw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gbnzsspiy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gefhtqzcd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gppqagfoi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gitgqozmk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcozawwef.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gfpfmtphs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaeendiwt.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gaahlsaba.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gfqguixjy.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gtmdvcers.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gjdscnrve.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblywtxzf.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gscovuyoc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gssftxyhu.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gzjuwbrgk.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/ggicpxdhl.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/guydrqrrd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gwgraxkmu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gcxotxkwk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gxnmjjwbk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/guxaxgqrt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggyborqmg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gjvmamaqd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gbwpapjuv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/genpttkdt.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gjxhlkxtz.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gtmpctyol.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ggaqenmzd.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdgferono.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/govxlwtmn.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gnxoklgfi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/geelnlxus.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/glcngwvhw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gdueeptnn.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/godlgmqne.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gwbolmuul.sHtML


<!-- 参考信息 -->