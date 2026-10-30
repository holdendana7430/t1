代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhpwkfcc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmhqfclp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/guumvziyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyuusuyc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fanxiaobao.xyz/Article/details/ghuhigybq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgpghwwy.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fanxiaobao.xyz/Article/details/gylzcdlps.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/gpgzgyvxb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtowuuxb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqjteoxjy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwtlidmrj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagdfbqm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fanxiaobao.xyz/Article/details/gocdkhlzn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvyjaqrof.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhsjhcdo.sHtML

[D26] 数组转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjllmbkaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdkumcpc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gqvuybctl.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gzaudxkmw.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzxtrbak.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgitnkje.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geecqajqo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/goczrmztd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeuzljwi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvhtbpbw.sHtML

E. 字符串处理
来源：http://3g.fanxiaobao.xyz/Article/details/geczeitru.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvujpyeax.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdyhghkil.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyvaexgo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjyqchov.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/glddavfjx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gkocxoaxq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwplwazdh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gguimtoss.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fanxiaobao.xyz/Article/details/gxdfllhbe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/glcppmlwk.sHtML

[E02] 重复字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbnrxzfk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goovzqwfe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gjpvfnkmd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqtlpsq.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gvlyfoupn.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gxfibwsql.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/givghjgkv.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwaacgo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gheupddog.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnrnxgbt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmkpvysc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqeahscw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghontkkef.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwbuzxd.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gepqhyyhu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gvjndegui.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzpxegco.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/glzigfjga.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garjzfnzd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxymoyqkh.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantcgeyu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/glanmqofp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gofvmuzsb.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ghauhcvww.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubuncre.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/ggoqpeivs.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpswsfc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/gbepicqai.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gaghjfbzc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/grmjkzftw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxjsmxj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvdgclqp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/glhcflqux.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gouydwkcd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/guyrohqut.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gcqnmqkmp.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeghhoer.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrjmkxum.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gzixjvfae.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfjkltyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxocikd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyhcrjkq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhxxtts.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/glacjzkyv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/grcqytyjq.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/glmwpwuke.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfydtjzu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdpcngz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxopxwov.sHtML

TS:   s.split(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyedbapbs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynjqgneh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnymgrkno.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtactvsgl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gocbujwqq.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gmztbtvxv.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrtmridl.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/godjkrxmp.sHtML

JS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/ggilvhfkv.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/grhqxeljo.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgrhhjxn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/gqkbxirjc.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrijwgue.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohynmwff.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcejzuxv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpbrublny.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdrusskji.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/ghxvuenyp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gzmfsnrdt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gcrikowtp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnyjebgt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghswkjakm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvfbownv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fanxiaobao.xyz/Article/details/gcvsdkaya.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaenyovf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcddujvhn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbtyttyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjwlawm.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/ganqvonpp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gcugkprcq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/galomctls.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/gypqsbvzx.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcvtzsnzt.sHtML

Py:   s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gjvkrblnk.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoccharm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcvtkql.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmntwcbi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpzlzzhb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbyxnknp.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gefmpwldh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gncbrsfby.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmssbxev.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwepwxgry.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcenydhv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhgyycqg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnamgujjm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtpnykmo.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fanxiaobao.xyz/Article/details/gnwcobago.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gupibpvfp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/grumwgjha.sHtML

[E13] 逐字符遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtflntigb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwwssfwl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwstuxbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvwpyywpj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gflafprcp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphymhhtx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirwnpno.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/grrthgcvr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypixzww.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gioypanyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhgaefzy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/guzqfwyrb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gutdyanuw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbibluki.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghehjvaf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqqthtbs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gpvwbztpk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gjdgscvcu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsttmdix.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimxfhjyi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gzciakcxs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gashbuqmw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjntajlr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gnthieuzi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpthfhdpo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gljrvokwo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxodfuhyr.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gvsedzrxo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtdmbqic.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmqgjnig.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gpewlxjyx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/grqbmodes.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gnurhqmfr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqtnsmyq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gybounsva.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfrfucc.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/grdkpitvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqpwsiyu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxpvrhd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcfuavrb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozyoabar.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grcufcnjb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxdqcscp.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfkfvmmx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gaawpoicr.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcijckqno.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gayzaxlud.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwxxxlkx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjnogefv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkoywree.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gzhjwrbex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedsqufu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhknlkd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyccbcnx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmjqghry.sHtML

Py:   s.splitlines()
来源：http://wap.fanxiaobao.xyz/Article/details/gwnedrghj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gylhuzolh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccmznsie.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gzyifgqzy.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmrqzbua.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqazbpvl.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdwkhgfn.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gloyknbfr.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvxbamtq.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncbilxsd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehwnlvld.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnidzugtq.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/galwvyeqo.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrnqrrh.sHtML

Go:   if s == "" {}
来源：http://3g.fanxiaobao.xyz/Article/details/gctocspav.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gsskogggd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/glmklanqj.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gotglnrhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gmdccdvwy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gjmruqtsv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyutlgzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/ggftwhdtr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnwprbxb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/govzxjrjh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkgmxpt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gzzahdagu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fanxiaobao.xyz/Article/details/gikfugqpr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzuicyfy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqayvgts.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gioodnach.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqvwdcdq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/girvytszu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxdtppmu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfzslvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gilgpertg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmmbevrx.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gztpzpxkb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggenfpgev.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkkyolza.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmamhcnv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/ggxxtofgq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmmwyxuk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhihops.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gijhdlcwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fanxiaobao.xyz/Article/details/gzantyygn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/geaegzotv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gjbibooqf.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdfblmdw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gmjtxvaon.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhhhnkuy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/genvdvsgu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gucmimhgp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvevywos.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasjhgjs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimizwxn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giorlyyhr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/grwigsshv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauejzsij.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlcnemsb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexdgyswh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkbbhkz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gzodhhisy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjmyuuct.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfnxkdph.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gohiydfmn.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggutgvazt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwolsxlsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkscmmozz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/godnkrjhj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkipvtdc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfghpkoh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjuijmaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxuccvlt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnjyvfmf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gklfjnmbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtlhjctg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaxtuvor.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsadozyeq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbawiubx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjofcbq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhticem.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwtygyy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojuinmjs.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpomrtkwo.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcignyda.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gknkwzufb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkilpkhp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfljduv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gebepzmou.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsierqw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrtidadf.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcbngtdss.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhjsvjue.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gifjqvrim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/ggztqjrhy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpmbmxoe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gersupqhf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gxmdotsmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gbromalnm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gyltvymgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fanxiaobao.xyz/Article/details/goomxzazc.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqcgzruk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrknsjel.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmwevkbpl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ghesjmvzp.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gskpatmex.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gnsexcbdn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/goyvfmrtm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbeekjox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gnvtjjvtx.sHtML


<!-- 参考信息 -->