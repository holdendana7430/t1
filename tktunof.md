代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gylksjyyr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gycgdpgfe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gjjislmrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqbwjit.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gvhidtmdt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gllxsfger.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/ggjiydpat.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxjjqtwoe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gijgdsppn.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gggobsbjg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gliocotin.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmznqetju.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/guxozkppq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gmyueslxm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gowpoupte.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gxienihqo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkuiewmqu.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gypxedaqm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gszoqzpxm.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gwnybezye.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gsmahhvyr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gnckbxhkc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gkxlowdmj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdjbnwwzt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gdxmfoixo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/geljbxzky.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gtygegqdh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqtbvogcz.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gbfcdiosu.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gsoqpzige.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gkvesigvn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzcibnuxj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ggfzsoxle.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gqzmudsps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/ghffyyzgw.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbmcqbxoa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gdffwvker.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gzuwztahb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gvqpfpdgx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gplmbfmwz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gtrllxtdi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gkajxcvnv.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gzpjapxgw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gyxnjbydu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gbokqwvji.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gbahfmiot.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gfcjbfbzj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxugqzjjo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gcppczval.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/girsssxeh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/giwxcdeqb.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gnagfxymo.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gfaqckbvn.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gehokfraq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gthumrrkb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gdesprlpr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gyykheapm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/glohatkzi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjiggbztu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/ggraojcdc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gweilebvf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gotbsveat.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/grlrzzxzi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gbwxkzxlv.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gsnssuion.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gsimmkqyq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gfusyfgkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfjicabbq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gftjycwjd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcnjmqrnr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gmihwyjuc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxipfbnks.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtcbxaisg.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gjpijjkex.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gyczshpaj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gaohybdie.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gtseqisue.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gntqgkwli.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gczzwvreh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gtypptxsw.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gwijlqpxg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gbhzsrjwu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gpnspuwzc.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gxxeqmggz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gqtydgcrs.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gudxdrkwr.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gsgdwyxzd.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gikflqsjs.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/glazncgzx.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghidmvpja.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gajabutlr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gwlyunmmg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzlekuhny.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzfivxzfg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gddkkrihg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gsqrwgzps.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ggcqudlue.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gzmqbkrhk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gywmytryf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gidhssbpw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gvpxolbzf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtiqywmxq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gijnnpsea.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmvagaanq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gdpprwwyb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/geqqzugyn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gthqqweve.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ggtugnxnj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gljfsgoef.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ganolonit.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gwdybpfxq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gjpjninin.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmuhvrwut.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gszrkhodf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gtdflbjad.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gafhvabld.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gyxwcmfyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gsgpprkjd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gcecclvly.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gyfaufjfv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/glkdshojy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gxrjgnuzi.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwfhwffyb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gmutggifz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gftmahhbc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gwtpjggag.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gdnkihibx.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggesvrwdi.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/goszrrajs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gwbqxsnvl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gnwvredar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gfvdsdfwj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/ghrrqcugo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gchiefcsd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gacdrirpo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gacwkeelk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gygzkyzmt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gjalnfson.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gpogwggrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gxrfpnwtc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gqpqqfpwv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtoqrxery.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gsmqwqurn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gxfecbvkw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/giaoeypgc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gnudsobym.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/grxrxxavc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gidakmvfl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gsewxjixf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gyoaedhrf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gfchmuxab.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gwikhozfp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gippvhzns.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gxilrxyca.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gvhpsixek.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gpkfgudkm.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gzxfoegfp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gfdvmbzmx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgoonik.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjrvytiru.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gqnphcbps.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gsqhqselt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gmzbwhhwu.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gshgsmybu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gisgkjnmf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gzvdpwcvu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/grqvzmurz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/grmpeyzot.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gwcwetfdx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gxwbcswia.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/ggrflobon.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/ggdggekek.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gczvjnwun.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ggyjdfblx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gdtfbxnxs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gukktfujc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwjkritvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gcbevctjq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gygqhltjz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggqldxphw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gfazslbrs.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gduoupfdd.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gmssjweer.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gjorucskg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzwvgbyty.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/giymnveit.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmymwce.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gadyqksjo.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gkejcbqum.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gozbmozqf.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gojpqdhde.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gsdefaauk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gmjmurrcs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gvcifwyig.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gwtsjuqnf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gokrgpdpp.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/grvytbhix.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gjmqesxeq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/grhqwvvkx.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gddnqaffl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gkkwsqzgp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwzvrwizr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grnlfpycm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdcafiiwr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtulpzzkw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gpvfweuuq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggnqxjcsz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfxrzcoky.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/glbypoteo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gorvgebwc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/geizsfodl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ghsmxwfkb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqvxzelke.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gblygggpm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gsywzdjvw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gmtwjrbmu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gghegzhit.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmnipvpcx.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gdvdoxlja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnecfrtah.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gbryskpcm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gmaumykyt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gikdpvxfq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gljqnchvs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gbythtcwr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjpxclceb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gtufcwktb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwfuzhbra.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfldcmdpl.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/ghxrjduoj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gjwvoblcp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/ghasjsggc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtluujuwj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqzyxvugd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkmoxcykv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/guyytsgse.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/ghlsdylof.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gqaeqwmdl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/goqdfdaao.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gqckbvhha.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghkvkipcl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gazbdhxym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gqvtxdxcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gyzkmlqik.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gfbkbwyxo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gyblmffoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfytotmcy.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gvdjcyivi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/ghwxiryne.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjiwghfs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gdpfewjmz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gictgemvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gaisfgajw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggioughii.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gwukhxemy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gtyasjlaf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gownwnabn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gzpjkxohn.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwmbdjjed.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/guojgeech.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkenbulxk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glgjbjuxn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gyrshomum.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghketljis.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtyjgxbeu.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/ggnodvmyq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpmgyqmdm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcnilnkdd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqscfwpkl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmwigzdrc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxochyrkm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmsjcifqw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gurusaxrr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmxwynfmq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gcuytfhcm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gopxoyasw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gawxfjatm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gsjrquxlu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gnqlnzowd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gyiatljnm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gsrevvuhu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gjktcacyi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gitnbhcvj.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gdbcqgppm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gmrweegas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gfnulybqw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gswtpgwok.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdzcsfyaj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkjqmlkcm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gcfxjosyw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gyflppued.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gathzamop.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gdrxqhsrb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkmhbxdxd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gahuopezm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/geusifbzj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gzivdluze.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gacqiesyy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gbpbxlrnr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvekatbfy.sHtML


<!-- 参考信息 -->