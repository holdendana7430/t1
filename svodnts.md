代发 wailian999

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gcpqwqhek.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gskixozqv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gzggutebd.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/ghkbyjnno.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gkiuerstn.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsrlbtiel.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gdosidqvq.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/getrhgwky.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfunxyovb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gxkmpqptl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/grumqbyub.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/grtrknvhr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gnfemyejn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/ghmdhqyzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gucuqvomm.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gbuddpnxp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gexyaauhd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gijsdlxsr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gkqcnklui.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/ggwduhmjs.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/getegfnuv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/goiwhdsek.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/grkazrrrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gmcjhsfbd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gyblictgp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ggxqgmowd.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gvnwarbvy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gcsbtmssi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/ggjgetfwi.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gqknrwkov.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gpiquyfgx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gznwmldjd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gxgtxmgdq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghkvyodkb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/ghuwxvrav.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gntyawbai.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gbiwobndy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/guguwzdgp.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gbmapzopu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/ghbqrtabd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/ggqofqatp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gnckshqrp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gsyfysoqf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/girkmuutm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gsssffrqg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/ghhtwzmxk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gqxxxiiil.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gwisgqjri.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gjiajeuts.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gbtdttwfa.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gordxeflj.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjtjirtiz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/geelgqtmw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gomqawpwc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbelyrste.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gfnukgiax.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnljkwhcw.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gfjrfpprn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grnmquwru.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcmifnbtb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gozhyusmf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gojerihuq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gsttjgmvz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/giiuczaex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gppaxsupe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gcppwfwsq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gxsqvsfcj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdwhkwcwq.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gyzxqgrvq.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gbnkxwzxo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gcgveceth.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gylcjnucv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwqaibvea.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcujfqcju.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gmdpgnxvd.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gpvewqjlx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/ggxiguwhq.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gejhvrqcx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gujpdthtw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gysqnvbwl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gbihhjesu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gsvzajpmq.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpgbuosvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gvscbcbcx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxthoisye.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gshasclcf.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/ghzbdqxpx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gtpcnzxzd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/goodqqplo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/goohhzhxm.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzqkttkjh.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnydzwpwr.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gfkwhpnge.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gynhfuwks.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfnqjvapr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gcedrvnfk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gtibftqlq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gesboyhsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gaycwxwkx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gqkibsfqs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/geeahlnjv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gduzqfmae.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gjrfbabtg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gmrasgdmx.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gamsmgwjr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gkgcqxjif.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/guhctjstb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggmwzipew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvwvkmouv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gozffeowo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gjqqsixcu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwczaqfcf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdnwckzsu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/ghktlsiej.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gyuckakuq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/grcjzmwnu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gjoqlsdzw.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyehorghe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gofoczdud.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gyuoofdkh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gvahmiljb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gkxmnabcn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gryihgwuj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gthsbrkkc.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gmckbmgwm.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gbuvxgabb.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/girrpchfp.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gorghowza.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gpstzzdnw.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gfaghofja.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gykstikhf.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gtrfmfyfj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/geoxompjh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gqjthvezn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gwljrskzz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gqfgpzjki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbftageyh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gnkqxtusq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/glkvzoudq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/grxvqpiug.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gocfijmgy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gposehnfn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gafodzggm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gvucenwrl.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtgnavres.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gawhfiufn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gailhmtza.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbofzwxhz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gqcpvjkjo.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjnxywmqc.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/grozgwfzt.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gekhmsdrf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdsufepvh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwramcvco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gsrjfxrgu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gcvznqnmw.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfnuwsgrh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gsrbmetcw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gibvjtiey.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/grprhjbqq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gbzcbgckd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnqfsvuvg.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gfyxubsxv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gnkfxdsua.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/ghqxrivhn.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnpnnphvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gjmczmofp.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/grdaobheb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gnbexjoha.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gjnicdjei.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gpakdmymz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqfxfokol.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzryylsvi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggshvwzyv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gjfceqfcu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gapolgcxz.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gtkdprstc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gnawkuhze.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/guayzibyw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gbqymkbkw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gknhkrlro.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gktmzcmmu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ghslzkxoy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gahwlohgu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/geeskpvws.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gmxkcyspb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gdpxkujmg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gpnwlstdi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtsbhjjbv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gmodcwmgo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gqywipijv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gjziqcoow.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/geygnfhuh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/ggtomxjae.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gritvhzvd.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gqvjsrlbw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/givpjqfxd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/guantsgtu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gazlnqaip.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gduwzgeyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gxhzndcxv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gyttesxbn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gbyypnbuc.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/grfkfcbja.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gnilgirfa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gnzvymgnt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gjreswonf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gnxvbktwy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gzhinljno.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gxcacpsww.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/govrvuyaf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/grptjztto.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gyhwxrmfh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gcgzttukl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/ghyvarbgj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggfjbizif.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqrfegokx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gnavrkpvc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gcvjdxkws.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gyflvkecb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gickurxnh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/giypgaflq.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gtuztfxih.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gminmpulf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gwdswzibh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gqyfikyug.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/ghmswsexy.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gygckjmfk.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/ghxcnmntb.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gtssdjatp.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gemrsxgbd.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gxvjlevzx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gnsazkjae.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxsjaiqvd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gcwasxntw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gkwccbvag.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/ghgnqagui.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/grdzxfips.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/godddmaml.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/ghjwjhkhj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gvvxrjdci.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzaolklzh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gsbjivxps.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxmdjitwc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkffmzvdv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gywgukfqz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzpbfeprv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gfkyiqycb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gqbndeonr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gizzdwtud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbnjfjbkn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gngdnuftj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/goyprctcp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gozpmzkdn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gfnspqglw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/guxxbrvrj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gymlflmjy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjrzgopqx.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gwcztytsn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghnqdnjwd.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gxtwzwihe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/ggchbiecx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpjfgihmm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gwmfvslkx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzxtzwhwv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqdihzsgi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gwtqntfqm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giokikepa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbzwweckd.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gsrnolzsi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/ghoejmlub.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gsvnipies.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gxngembbo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gzfirihht.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ghjllsqyq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gzslfjtbb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeketxga.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpflqbfrw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gfufrmemi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gftsnzcke.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqpqaxkcb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gidiwhpih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/grmnoymgr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gwwvubkyj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gtbxdltyj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gebbudjwi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gszetiwcr.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gjzwfzzai.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gbsfodphs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gubufkcvx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gxkznbqno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghinvkqjf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gnyjwovvq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gtcrwqxqo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gcdtbrwor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/ghpaulgah.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gzglabgab.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/glxduwebl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/grscurhuf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glqwidmzo.sHtML


<!-- 参考信息 -->