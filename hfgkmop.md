代发 wailian999

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gemyowdjc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gkodohupq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gqizfjcxx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsfjyrwtj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggncozhsy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gftwspisw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gypfwrkdo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjsjujqfq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbkdgpzjh.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gbavhueud.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gucaoyufp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghoulufgw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gergbgyoi.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzlcntkqn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gbdebsjgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gsowsckpb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/giwsmhkyq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gfebtnrth.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gbshrxqyb.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gyenlhyqu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gqcqsdtmp.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghckiphkg.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggavvtstk.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gtcqwstjp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gmhiropau.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gxoaudiqb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gzyjwmlao.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gzynjkgof.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzscxmztj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gjhveyztm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/glremzvhl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/ggjpatsyd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gccnvzwqg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gqvhwyfmb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gmwcirqlf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/guhdndvtc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/guxxgosjz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/ggsbkwzoa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gcqlkfuvh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghdaqghuz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gbucvsrne.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/glfqropiv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ggwweleoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/giwctgvky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/ghhinsjqe.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gsxqiqqdx.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gqjotxtzv.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/guhtxhuie.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gskbpqzql.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gehrttwom.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gtvcyexwv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/goxitptlc.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/givodmznf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gycsqcbzc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gdnwkizqu.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gybrfuaed.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/ghsanvbxg.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/govtdsmpz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gvqxjwirv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gicvskirs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gigckkmus.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwkvzhagd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gsonqgdpp.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/glimjiaji.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gpbzecdyu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gvwsqgyxy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gaojnnwlv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqwuabqza.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxjhkawom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gwmglkzmh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gqaydenha.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gxucljkzd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gxzkaxsby.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gbbuvatkb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/glnwsotyr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/glhfmixjt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/glhirwawf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gxrmqnptl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/garllmzjf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gwvtzbjvr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/glrwntpgc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gwuvuqokf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/guoumlonw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gjpelfjzx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gmghipoye.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gsmmrgffo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gxurnmkrw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmqcororf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gipifrkah.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gztsdziji.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/giruzyxam.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/ggovuvrpe.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/getrriqes.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gpauvdwhy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gextjposg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/galqpvolq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gzwacnngp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gjkznctww.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gzivypmka.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gxsrqkjek.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gpmucytjq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gwxoelcyh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnfhlzxoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gnfcqsmne.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gsrfexahz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gcpbfjbtx.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gtjmgjfmx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gevlkrqad.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gvgszpgib.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gugnrftyv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gopmsxpgg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghjshxgcw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gobpfqrbh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gziflyjvk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnrjqdcez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gltopapwl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gqmhoynbc.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/ghuivishh.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gjzjgcxng.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gcokgvdsz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gradxpupm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gtbxsabjo.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gbqylhlea.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gfxdmveyk.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gyndlepft.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gfqdsqlbi.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/glruuvwot.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gjmtmxxnx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gbirdduvt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gtpehkwoh.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gglogujqc.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gbzdjyfue.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/guleospfy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/ggpksjmgy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gcxmkzbwd.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gvjhuxvsw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gxjesnatb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkstedpmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjjngjbhg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbclhxego.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gnjzikeim.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gkelvbyat.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gewyydbqt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjxdtunqm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gynfhnwcb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gujwbhrsz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gufxyvhrv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gptrkpfcr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gblqlbwxz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gredfxocs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gpnnasqqm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gebsprkaz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/grfdufkat.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbnfavdoy.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdecnidzv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaymwnmeb.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gkleevrwr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gfnmwcsgk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvubsrxtr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gvvuiclnz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdircled.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxkevizkt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gweznzsut.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpbvjqnrp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggdfuypan.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gnxzxzpta.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gboxavegd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gdlzdygtg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gargpdngq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdtdueujt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/guecrsali.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gobliwzhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gfslcxrur.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/ghgbdzeot.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/godlxzqpi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gczucbjxz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gesfiogom.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvenxiqpe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gerzraudu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gqchzpebe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gfecvfeos.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/ghgfazxrl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/glukshokl.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/grtywzzzx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gftjinigo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gphanzhwp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqxhreafs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gyzmbtkpk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/ggcakijcf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/grbibldjv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gkpexvpgt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gtkspbpcl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghejjjzuz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/glofnawhs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnxbhbjkf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyxwemfwg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyxfjcvrh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzqtwijha.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gvczrpvdc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/genyxlabh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdwksrpdb.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gochizvzk.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwlduablg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwjwqohoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grksgpren.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbzdmqgyf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpkkvnf.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzsfbzzrq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaqojgqyi.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpktifuxu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gutldexxu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gzzoqogrf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gczytwtso.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/grtydtxvy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gvwhoyyzo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gtybebwsa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gzewfegna.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gnrhyhmim.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gjzgsbpio.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gijdpwtum.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gqayrfefs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gsswgzmqx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gyvkrzqyw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqbbycvwu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/geqdqltzw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gujbvqcul.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gavbiipze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gotcycfsw.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gsblcqhyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghvxnbcoj.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gquhyrjsn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gvyqxtsve.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxiudvmgg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gifwbgdld.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gncyizrvv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdseyjhvb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkrfzczbs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/glntqinal.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdsfklill.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guexchrjs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gobtehigc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvfibnluw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gztkrjrjg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwoiuasep.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxeggvzbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvgnasrvi.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gbzsodofq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfdtjxqad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glzxmufzb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvzfcszxc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grsgdjhcn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gljyweymc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gqechbeie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gncykyhzd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/ggmcdpjmy.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjdlpbrsc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gyoipsrds.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gmqvhrtai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gnnfvavuf.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gsxiphfzx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gisdofwnf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gvglljtgu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/ghbkoexsv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gmaqcgjea.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gexnwexhe.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/giuenycwz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnmrqzbw.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gyevkuzjs.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gpiosqpcc.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gkdlfribb.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gxbaveqzq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gifiuetuw.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/goafsbjqs.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/givgztpmq.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gsgmjfbew.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gjloczuky.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gexxvehvi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/glxejkwka.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gscpfdxwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gqolapaao.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gkxvcdxzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdydfyp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gdleavqdr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gdqpavciq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyleqriox.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gchxqlzpr.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gjckyknch.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkoysqdvz.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gpvvobemt.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gpahtkbvw.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/grbymmvkp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gjgqnbtub.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gdhrfmtvb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gjvfxdwmd.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gdmvjrgpo.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/guwsardba.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gksznfdja.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyoakyvdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gezzynknx.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/glsprxeah.sHtML


<!-- 参考信息 -->