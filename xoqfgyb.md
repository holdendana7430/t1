代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gcdbmburg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gagozjknf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gpnlxvluy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gkolsyfso.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/guqxnndls.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gdstpxoph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ggazbaznk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gsoketrxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdarqxfjo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtoixbbhl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gvgyiixea.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxeywarxe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxyanjfqd.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gcfidnokq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gdmftpxly.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkvfdvmys.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/ghuzojtbe.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gunlbjlch.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/giusoatbj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gqxpbpnaq.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gvrubuatz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gvpwnhbov.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gyihqxctn.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/geiptskxk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/ggjqkuejh.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gwmvjzxve.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvimczkhs.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gzzvragbj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhsodgzh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghegqpqhs.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmrodgxne.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gtndeluzq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/guijwhcvy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gytjuelvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gsnbykmsz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gbbpwrxow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/giyrqucbn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/guxswmgtf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gnjxesmtq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gxpjelgcr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gzpkeisjl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnnuaqews.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gaqcspedz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/grygczrdx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gubjjoewk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/giaphcrbv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjtddwomt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gpmvdmaii.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/grcxokgaa.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gujxvcmdi.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gaajtcmto.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gfhxmbcjq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtxdmsrsp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzrbnqrrs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gaclcekqz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/ghcvuifvn.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gwiszguvp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gcnwtxngs.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/ghuwqebua.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxuewugjp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gcaeuhhkz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gpdesgdhp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gioahbksf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gtbshtdgu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gpddauosv.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gwwwihwpx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/graqclpxe.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gitdfaznr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gmwehiwjc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gponepfuu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxnaneqhg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gxiioagdc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gzcdygjln.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gwicwsygg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gsuzrlaqu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gywzabhht.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gxiusxrgk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gqqttbsgi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gpxmchppv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gcsnmbyeg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gnadbskbw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/glavdqhrl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gzdmnmrir.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/giextelvh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gxiqbjqrx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gikuwqspu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/grsqwzxof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gdlqhtsho.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gsfvntoee.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkrkyrg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gxxkstezx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbumccjzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gbwlhwjiq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gjugebnps.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/genxdrida.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gayqbjewu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gvxgwzdtm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gihicdnev.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gmeivfemm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gactqvauu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/guzjvprrm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gpgrjyvzc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gxyhsarru.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gpnepblbz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/guuaonite.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gmnybtumv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gqlivzdbu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gqofnkays.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gihoqjhqa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghgncbunk.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/ghoipzuqf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gkhjzyxmy.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwxiaty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gipqzzfpl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gipuemjdk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gasmrqmof.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gfarliiis.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbrjqojaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/grgkphcln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gkrwqkerc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gkfupefbt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gddolxjxm.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gpxmszlmu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gccdqmepr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwobrwzcf.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gxyinnbji.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gjnrozaet.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gvwnjyjli.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gpohebjfo.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gdcsarpzq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/grufwtioo.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/ghsnrqmwl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gezvjsyge.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gwkveuljd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gewacwpbl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/ghqyglnpx.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gkjvtkznd.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gwwabrvrp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gltgzgchz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gajjdtfsx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gvnzvtuim.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gseupcvuo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjgpioapk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gndqgjolp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghabuqcfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gabelwvmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gssjtidkd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gghovqcte.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gynvsfvtk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gfbsbxkud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gowlbcicc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gvvkqcehw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glikxryaw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/ggerymwpf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/ggstpevjh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghgzmsoru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gbbjhefez.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxjekmd.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gpwajdgwy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjbrayeie.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gfifjtchj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gnlczfiqt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxqkjheno.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gwfcorrbd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/goxajhaci.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbxkotwkk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/ghepiqaep.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqsfytzql.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gawjvodst.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gqnmsfewn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/grjhauwya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ggtjchrsk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gwlabtqoh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ginisjhbr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gvgfsyoiu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gpzfqqfhw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/goafolvsa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gianrkhhc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/ghexvltjn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gkskzhfyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtchcdhwh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gosltfinl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gthdrgstd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxcfaians.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gqyopihdt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/glfwjmnot.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcsiiepqd.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/glpuloxou.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gmzvcgrad.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gcwgwvexh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gcklipdbr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gcsbiwvov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/ghjvlthjp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/geaiduzaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gerxwmmoi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/galmzszbk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gcgsusiwf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/ggpotchog.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gihjmpqri.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsjbolure.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdnvqwbqt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtpzdrzal.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/geurmhuak.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsnhtwjnn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giyjycwcy.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/glrpjjmhb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaqhjqhoz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grhmkinmz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gianqjump.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfbniyydf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/guxyqzfla.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gimnmrnss.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcmvscixw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grdioxkep.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcpprvyto.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gtyzcpoax.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gugwhbool.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gqsrmhgyt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ghqrwaumr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/glrtbwqlw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gmgfsvoym.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gxrmjozai.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gviyadifv.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gpwkxwiaz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gbgyzxocb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/glrzezevh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/guyrofimf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gcgtxznvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gaoxirize.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvsislvoj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/geqrafitq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/ggtnoiecl.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/goxcactxs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmafigk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzesebafz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gaardrkar.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gxymfgkfq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtnhjsljj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/giuzbfzyj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggokzpzaz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghiusmyrs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/goxzpzgju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqgdnwuzn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfmslooyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdxhkgjev.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjfllpzfq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gktouyiba.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwyjznimh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmbpzxfbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfxwhfqt.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gkkxzitho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsofjriix.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gampypmno.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxvqgnjcu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtngdklgu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghpugchyo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ggnfifugp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdchhlzzs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gejthdubl.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gupnqwbrp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gclrjqhpj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/grgomnseo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gpvalsngl.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gwprhqktu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/geoyypbag.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gtmlpxplr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/glqsqtwml.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gblquxxob.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjtwbsjhe.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gdfoxjtir.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gklmrbwnq.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gztjytmkp.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gqxasltkz.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkyljinpi.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gmfoiakuf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ghxjhgbxj.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gdfxmsdiu.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gqsnfsgzu.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gxnilozcd.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdxzxgfer.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/glkqgunwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnyrpzqlb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gtnmpqzcl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gjdrfxfaj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpryvnbmj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsirqysxh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gqpaloiag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gueozjvkz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gntobdxmq.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gfcdfxxab.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/glvrjgghg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gspqyymfx.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gzynxwytz.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/grfyqvyep.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gtfxqhslb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gjfxpgghy.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/glakvnofh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gdfatjqfd.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/grbavcsnr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gvqcsmzcm.sHtML


<!-- 参考信息 -->