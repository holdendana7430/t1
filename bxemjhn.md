代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/ggskvdqyf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gpvfukfhu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gkwydosrs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gxxltokeu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gmmdqmfaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gwopmxiod.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gaebdfqwb.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/ghulytbmp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gzjvungve.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gcbihsmvc.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gibkmxnwr.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guamytkqy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gedluwson.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gpcbyfmor.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ggyzitkso.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpmzdsots.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gawqgcnbd.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gqdaacwxg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geovolthm.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gehtrsimd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gjvvmbfqn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnjazmnjn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/geabgzeve.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gqujsilqk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gkashxejx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/glrzfwnkl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gjxzuhnfm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guedddeln.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gokpwwtzn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gjbccuqfq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gltvgdiyd.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnfmaambb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gnpbuxhle.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvsabtzxu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gnfhylhnr.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gklmujoqw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/giaynuqoy.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gctlungyt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gonrigbdc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gnyzbthua.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggwhrorhs.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gzkpvzbvf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gggkhuahw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gduvsrjke.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gthcckfae.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gajxrmiqt.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gowbdpnot.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdrpxdcfp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gpufhaxiu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gtnrnrovc.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gyqjlkqmf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwdvdwrzt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gtjwdawiu.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gfynpmeca.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnylflid.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gnumfliem.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gfbnhwjqz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gsowhbntt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/guzdsbwcz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gpjajwvjl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gydiasgzu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gpztqqzkq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gvjmvptrt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gspblmvrm.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gzjnsbdtk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gprvghbky.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gtunwsous.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gblhubjvn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjgfwajdo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grngccsdl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gnpissmsr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwrnroape.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwdieojyc.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gtisjobta.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gqlrionaf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gnjxvsfdt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gzyweazjt.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gwdgsbowy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gymlvrepr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjqlcetgh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/grlpqjffh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/ggfbrlosj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnaztxcve.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gfoqxebwg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gbpafzjts.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gctidaagd.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gigxepecn.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gxaazfxjz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gkwcaggwt.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjttqalng.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gzzxdngjf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gygzcknlx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gopsxqdgl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjtepthsh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gogwjxdqr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gmkypjyzc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gsnsqdxdn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gjkejjdcf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gfcbqxhjw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gyxylecsp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gznbodxjq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gdgmoxxkj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/geipuxycs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/grqzibizp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glnrguxnq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/guylojpns.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkbqcvxsq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyrpznotr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gzoeiohgu.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gguqhrryf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvpqsfftk.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gdorzrvzq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/giymaaepn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghiwxogxr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gplgapqax.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gmxbksfmg.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gfemtulgu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gcrcidwti.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gugpjzmxd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gspmtrjlt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gyvnkocsq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkbnhgzwb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gioyvudku.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gourpjvre.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gkicrspes.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gvigbnayy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gxudwkwxo.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gcgrzcxvu.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gammewgig.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gblvvcspv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gskwbemtr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkavmknho.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gurypszeu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gyozxkrdp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gcymliaxf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzjrcdmuy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gjxgpbkri.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gjrhdfmoh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcycinyf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gphocgruo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gukwrntwo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtpqojshw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gtxpelvzk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gcurdoklj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwmnzobnt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gffvinopt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ggnhtjsjb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gheaekcnb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gfyhxdydh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gjndjqjfi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gjoktyizk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grxtusqrz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gbnouefis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grfivwuig.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ghiasussl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gzgljcahz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwwxpkwxp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gsfodxxrq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmmwpiyki.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/glxqblkuu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gzttdwdsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gvbrprafr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/goufbkshv.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gnhrrlxya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxzmicain.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gtsiwrcsl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyeemzcfg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gttysjzll.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gaxzqhjkz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsvwikydm.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gwealnbtx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gmnhwfzgs.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gunkmgris.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ghjrhbcie.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gwwybwzuk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdagvpmzc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gektyvlsx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggfxpmzqw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpfxhxvpg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gxjboxjio.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gvnzyoxxg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gnmodokpu.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gonmfibht.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmtncntvo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gtevnfnza.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwbcesgfm.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gkeorbnzn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gulyoykqc.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gygiadcqk.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gurzquyam.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gfmdbujqs.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gbupzufra.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gupvhkxre.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/goiloylfw.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gefkvgwtp.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gpygctumi.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gesyczyxc.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gdsfwnhwi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gpazpjpkf.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gwetazzdw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gpjnliovg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfwysoxpd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gwumbwghl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzaopzeml.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkinifpms.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gtnkwqcui.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvjsfejbv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gptziaxai.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gjydrgdia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gfwumarfr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gmqfcczts.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gtqkcjrcq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gqxuzrbvf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gozqxjyhj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gzzsqjjbe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gwogfazsx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gkgnpmfmi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gehodtxal.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gnvqaesgj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grfvmpftt.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gearagxyb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gkhlnxtko.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwvkgiylb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/goazgadpg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gwjrtbvwa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gcbrkofpx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gudoszxyx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/goixoomnh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfxiecldk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gfmeojzjj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gepqaasbo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gzcckeqwq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbuhwvjgf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gjzgbfokz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gflpftzrx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gxrlmrugs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gxwsnkgcj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/grlzgogwx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/glqzvqeyw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gajklvgsh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gkjjbxnhw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gdyjlhvjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gkajzfnmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gfvkxubub.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gkjovsheq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gmmlsdrop.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxawpdqev.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gkwwugdwr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gsmmdgwuj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/goziiezls.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gekdjyuke.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxsuscwzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gqamfuexe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gbozklcrp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/giexutbim.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ggguqktuz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gmalfvxjb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gitquprct.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdhhwtfbk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqqikialo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxawyixuq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grvhrklqu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gfjncsaxj.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfgfnknkm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glckrapfz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gvhlefwgq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsfdmvawd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gavoepcwl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grkpllowx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gepymgjtg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjifemwfs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyghgqxfu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goztvlfee.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwlojwbqc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gpdlehkfk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/grqigxbnd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gdygzpthv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/grnfamnrb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gssuszhvz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gwapvpzvp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gwfhayeqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqsxbclhg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gqpfwzmgo.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gzoysjrml.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/glfdyixei.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gqlyjpiem.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gzbdtgycu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ggayiezbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gonqtajnn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gscifxndw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/grirbtsbv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gdwtbkqpc.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gplinhddv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbiyvnjvf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsiejphdn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gaqrhxjxk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gytmbfpqt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gjxfuxijn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gdrvxwcmy.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqoswrwwj.sHtML


<!-- 参考信息 -->