代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gezqqhost.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gkptnywxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfljsdbez.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gieogwqza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gahrmwtua.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gevfurbkg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gngpwsmfx.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gwjmaytud.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gwcaxqpoy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gqbpokzqs.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsgnlirqv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/grlehxtna.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gapahhzun.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/grqmrwxuc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbdqxmxua.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsmnpkhwb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/guxtxbiqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gduykfsrm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gjhqggoil.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gobadctci.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gmvnbomdj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gxlgjavvf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/giquishdx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghgcgmlxt.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gvbgxubjk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gqnqnhdeo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gvwxozqhm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gcipapshk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gcszwnqzw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/guwrmviam.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/glspaylby.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gdgbwngoo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gkjeefqda.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gollwyydi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gbaxkhvnt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/giyfqvrrg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gmvqlwcva.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gkrnlcumd.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmxebxxqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/giukkxxeh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gpdrohofn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gysfmbiza.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gyxngkxfy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gfojbeaii.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gdsogiryn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gbkptdmrj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmjsidgys.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/guwzocxit.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/grhuhhicw.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gegxfuvth.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gtdmfcoea.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gjktytgtv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gzrinbstc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gwuglovja.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/grvgdwewl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gargnollo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzxqzxxii.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gqjgtbydv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gwmhzscew.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsljblhql.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gskixndad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gruvszbev.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gtyddegui.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwcwwcgtg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjmvneuct.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gqcdvwquw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmgzgdzmx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghyuwixyj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gewistlbd.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gevkcwcpz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gparhgbsh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gulspague.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gjpvprpan.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gvddnbxqf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gewzutmly.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gpipsbieo.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/grmgukyfw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/ginecvrcq.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gtvneoekv.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gudtiusew.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glfspwaph.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzcacnmxd.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqlesjeaf.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gpibnpqrs.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/galkbfcwv.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gepeueeyh.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gsswfhzee.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gqufiyuqa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/givgzuwio.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gyiuezlpp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmwgpmn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/geelytwlr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gwvngwlxs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gvquminmr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/ghhwdvnxi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbahzcb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gnmhtwhfh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/geaexuofl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gbgeweaej.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gldnnygbm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvcbkrlrx.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gxwfciqne.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcnhkqbov.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/glywgqbjn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gmqhtciqn.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gkosjwcob.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/ghrzdewdv.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gfkgiknkg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gicmjecyr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvollhxjf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gvupiskbm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gvnttxiwx.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gxgvsyfjh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gtqvmhmzp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gcsxedvsy.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gjftprggi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gihypchpb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gtwvlnmeu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gxnzjkzkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gdpkcwqik.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/guzwgxuhu.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gqxkhhhbl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/glenauprn.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gexifwqni.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gbpxnswys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gzotegemv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gwdxaaebx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ghfbpefvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gwwpgqedi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gelznxjjk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gqzsazoxx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/ggpdtkhvm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gtdpsyjud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/groqapmtm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/ggwbzcwnj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/grgbxgsdm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gcptwmrqg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gjdotiyrb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/guswenalo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/guwdqpamp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnssqpnal.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gzqwfluyt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gfjtlljmx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gysufmzbd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/glivvjzlz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gakfmqkll.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gsdownsbs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gdfoelsog.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/guzwyxalo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gszslejwt.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gwojevytk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gsrzapmbb.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gfghnzgde.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/glcztuksb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ghjdgxbxi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gwyjgdeuk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gjbubzbcg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gurdmvyys.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/guvuxjnov.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gziurtwap.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gcnuwcfpg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gskxrzlap.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjhrwpixw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxkbaiunz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gqqkpaheh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gqbjpehjp.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/goakgxstz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gezgpvyrk.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gmhijviki.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gblhxjtat.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gznjqogca.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gecoyficx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpnbyyqrl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gazvfkush.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gomegwixl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gpboskllk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gsrkdchxv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/ghfwwzjhm.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gafewrgem.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gpyjpxzwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gwqnqiqhu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gfirkjuud.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gqjpguzis.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjhohbznr.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gdnhulstk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gyyqelnhv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gplnzirxc.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gixxgtqbj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gywiyfxvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gxrrlhhkt.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gfhulrirj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnrviafll.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gjipaachq.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gzgvdxaup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gjcpcvpxv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gnqwbcfpx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/glhwoqjps.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqixaecet.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxzaefebp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvimpodhq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkwspezbm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gfjjzsvhs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdbtqivut.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gckubtyxy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gjdrboohv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gsfsauiah.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghmsmhrol.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gfhrbkzbm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gyspkvxtf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ghvntklvd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/grzrbkhcf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpeyweues.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gsbhvggzh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghlpgbbal.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gcydpcwpq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbsewafza.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gshzgsvvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gpqgbamns.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfhfccfqn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gedgslizx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gypzlihyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqljwfejj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gjctkszpc.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gggnbmsen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmmvmdxee.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gxjgcnhtp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gcrvubmvn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gyarhobwv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gopmmagdf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gmvfgqxtw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ginvmylqp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gyrvmhjgv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gukbfosaz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbknerf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gxxacfnog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/glshpxysf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/giglhbbrl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/goycycfzc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxpwhfana.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gypverlkw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gxrtsymgm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gchkyricu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gylpmsouw.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/ghyeuzany.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsjbxvqhc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gxencywsu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwgiqeecm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/ghqhcholr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/grqwxuxvw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gckikreyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gubnprovj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gjcctveen.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gdqyivcya.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gyenltpob.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnkanazrj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvxmachlx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvaogymdx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtijfkiwq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gnaevmehc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbifkzd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmftvue.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/ghimgumsc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glhhpvazj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwltmznph.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glkajytqj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyidcfltg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbxyarfjx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gygzrbbwt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gngttxhxd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsonczqjs.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gcyktygjq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/guaukobtx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gxpbvknch.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gycpwitvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gvcjdqssd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gxnjinkwz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gugjeiksv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gvuvunuxw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/glxfprfhk.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gyzbxphvf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gryuokbcx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gehfpphcv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gojbdmhzi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gnstxqfcr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gfegywpbj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gutuuuweg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gdoinyoye.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gnrrycodt.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gfujmnais.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzjtzxoad.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gudtvwwri.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwlhpxeco.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gntpejmjz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwlppwfpx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gpsvzjijj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghnqyhpyy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ghpexwskt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gszsdmmsp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gptqgdvcf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsssrspwc.sHtML


<!-- 参考信息 -->